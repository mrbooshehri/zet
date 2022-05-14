# Check UDP Connection between two nodes

On machine A:
```bash
telnet -u B_IP 123 
```
```123``` is an example port

On machine B:
```bash
tcpdump -XXn -iany src A_IP and port 123
```

Tags:
```
#Network #Connection_test #tcpdump #telnet
```
