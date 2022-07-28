# SSH port forwarding

## Local Port Forwarding 
```bash
ssh -L local_port:destination_server_ip:remote_port ssh_server_hostname
```

## Remote Port Forwarding
```bash
ssh -R remote_port:localhost:local_port ssh_server_hostname
```

## Dynamic Port Forwarding
```bash
ssh –D local_port ssh_server_hostname
```

Tags:
```
#Linux #ssh #port_forwarding
```

Related:
```
* https://phoenixnap.com/kb/ssh-port-forwarding
```
