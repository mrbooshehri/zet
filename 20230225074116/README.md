# CPU usage status without top

```bash
ps -eo pcpu,pid,user,args | sort -k 1 -r | head -10
```

or

```bash
ps -eo pcpu,pid,user,args | sort -r -k1 | less
```

Tags:
```
#ps #cpu_usage #cpu #usage #status
```

Related:
```
* https://www.cyberciti.biz/tips/how-do-i-find-out-linux-cpu-utilization.html
```
