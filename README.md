# Whitelisting any unverified program

1. Whitelist the binary for next run

```
spctl --add <myprogram>
```

2. Now run program

3. The system will still prevent its launch, but now you will be able to choose "Open"

4.  The program can now be opened/run without any restriction

[source1](https://github.molgen.mpg.de/pages/bs/macOSnotes/mac/mac_procs_unsigned.html)
