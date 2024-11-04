# Recover free space on Linux

1. List of deleted object using `lsof`

```bash
lsof -b 2> /dev/null | grep deleted
```

2. Truncate deleted objects to reclaim space

```bash
find /proc/*/fd -ls 2> /dev/null | awk '/deleted/ {print $11}' | xargs -n 1 truncate -s 0
```

Tags:
```
#Linux #lsof #deleted #object #deleted_object
```

Related:

```
* https://serverfault.com/questions/501963/how-do-i-recover-free-space-on-deleted-files-without-restarting-the-referencing
```
