# Find and kill a port in windows
To find the process
```cmd
netstat  -ano  |  findstr  <Port Number>
```
To kill it 
```cmd
taskkill  /F  /PID  <Process Id>
```
**Note:** ```<Process Id>``` will be appear as the last column in
```netstat``` command

Tags:
```
#winodows #netstat #kill_port
```

Related:
```
* https://www.revisitclass.com/networking/how-to-kill-a-process-which-is-using-port-8080-in-windows/
```
