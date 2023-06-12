# Add timestamp to bash history

History command without setting the HISTTIMEFORMAT displays only
command# and command but it does not display the time when the command
was executed. So, to display the time stamp information associated with
each history entry the HISTTIMEFORMAT has to be set.

Some `HISTTIMEFORMAT` formats:
```
HISTTIMEFORMAT='%d/%m/%y %T'
HISTTIMEFORMAT="%F %T "
HISTTIMEFORMAT="%a %h %d – %r"
HISTTIMEFORMAT=”%A %h %d – %r ”
HISTTIMEFORMAT=”%A %B %d – %r ”

```

To apply timestamp to the history file add it to `.bashrc` file

```bash
export HISTTIMEFORMAT="%F %T "
```


Related:
```
* https://linux.101hacks.com/command-line-history/display-timestamp-using-histtimeformat/
* https://www.cyberciti.biz/faq/unix-linux-bash-history-display-date-time/
* https://www.geeksforgeeks.org/histtimeformat-variable-in-linux-with-example/
```

Tags:
```
#history #timestamp #linux
```
