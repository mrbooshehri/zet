# `cp` and `rm` commands in `find` command

```bash
find ./ -name "*JIM*" -exec cp {} $TARGET_DIR \;
find ./ -name "*JIM*" -exec rm {}  \;
```

> **Note:** Use `\;` instead of `+`

Tags:
```
#Linux #find #exec #cp #rm #; #+ #\;
```

Related:
```
* https://stackoverflow.com/questions/12060557/solution-to-error-find-missing-argument-to-exec-with-find-exec-cp-targethttps://stackoverflow.com/questions/12060557/solution-to-error-find-missing-argument-to-exec-with-find-exec-cp-target

```
