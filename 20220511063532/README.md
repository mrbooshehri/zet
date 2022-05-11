# Run VirtualBox in background

```bash
VBoxManage startvm $VM --type headless
```

You can also add the following lines into your ```bashrc```

```bash
VM='anakim'
alias vm='VBoxManage startvm $VM --type headless'
alias sshvm='ssh -p2222 localhost'
```

Tags:
```
#virtualbox #background_process
```

Related:
```
* https://superuser.com/questions/135498/run-virtualbox-in-background-without-a-window
```
