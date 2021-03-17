```
{ cat all-vsd-layouts-split; \
  echo "PASS2"; \
  cat all-vsd-layouts-split; } | gawk '
function finish() {
if (pass==1) return;
print vsd " would explode " shared " / " c " blocks"
}
BEGIN { pass=1 }
/PASS2/ { print "Pass2 starts at " NR; pass=2 }
/^VSD/ { finish(); vsd=$6; c=0; shared=0; }
/0x/ {
if (pass == 1)
{
        # first pass counts the number of VSDs that reference each address
        match($1, /([^-]+)-/, m);
        ++counts[m[1]];
}
else
{
        # second pass counts how many of each VSD"s blocks are referenced by other VSDs
        match($1, /([^-]+)-/, m);
        ++c;
        if (counts[m[1]] > 1) ++shared;
}
}
END {
finish();
print "Pass2 ends at " NR;
}
' | tee rebalance-impact
```