# Cluster Drive Rebalance

1.
##### Note : This may take a while and you cannot exit (ctrl+c) out of it
```
sc vsd show display extentLayout > all-vsd-layouts
```

2.
##### Copy the following contents and save as a bash (.sh) file

vi [step1.sh](split-1b-extents.md)
vi [step2.sh](measure-rebalance-impact.md)

3.
```
sc replication update enable no
```