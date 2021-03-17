```
cat all-vsd-layouts | gawk '
BEGIN { mb = 1048576 / 512}
/VSD/ { print "VSD " $0 }
/:/{
match ($1, /(0:.*)(0x[0-9a-f]+)-([0-9]+)/, addr);
c = addr[3] / 1048576;
if (c == 1) { print $0 ; } else  {
 for (i = 0; i < c; ++i) { printf "%s0x%x-1048576 %s\n", addr[1], strtonum(addr[2]) + i * mb, $2; }
}}
' > all-vsd-layouts-split
```