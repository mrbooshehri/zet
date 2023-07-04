# User variable in for loop bash

```bash
#!/bin/bash
START=1
END=5
for i in $(eval echo "{$START..$END}")
do
    echo "$i"
done
```

Tags:
```
#bash #script #loop #for #variable #Linux
```

Related:
```
* https://www.cyberciti.biz/faq/unix-linux-iterate-over-a-variable-range-of-numbers-in-bash/
```
