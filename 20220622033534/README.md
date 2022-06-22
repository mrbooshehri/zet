# SSH to termaux
1. Install OpenSSH
```bash
pkg instll openssh
```
1. Set up a password
```bash
passwd
```
1. Find your username
```bash
whoami
```
1. Find your IP address
```bash
ip -br a
```
1. Start ssh
```bash
sshd
```
1. Verify that it's
```bash
logcat -s 'ssh:*'
```
1. Connect with other device
```bash
ssh <username>@<host> -p8022
```


Tags:
```
#Android #ssh # termux
```

Related:
```
* https://joeprevite.com/ssh-termux-from-computer/
```
