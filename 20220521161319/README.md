# Get specific time with ```Date``` command

```bash
date  --date="STRING"
date  --date="next Friday"
date  --date="2 days ago"
date  --date="yesterday"
date  --date="yesterday" +"%format"
# Get yesterday's date in dd-mm-yy format
date  --date="yesterday" +"%d-%m-%y"
date  --date="yesterday" +"%m-%d-%y" # US date format
date  --date="yesterday" +"%Y-%m-%d" # YYYY-mm-dd format
## store y'day date in a shell variable called yday and display it ##
yday=$(date  --date="yesterday" +"%Y-%m-%d")
echo "$yday"
```

Tags:
```
#Linux #bash #date
```

Related:
```
* https://www.cyberciti.biz/tips/linux-unix-get-yesterdays-tomorrows-date.html
```
