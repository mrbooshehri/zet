# ssh public key permission denied

Error:
```
Permission denied (publickey,keyboard-interactive).
```

Fix:
Change the following config in `/etc/ssh/sshd_config` and restart SSH:
```
UsePAM yes
```

Tags:
```
#ssh #public_key #public #key #unlock_user #unlock #user
```

Related:
```
* https://unix.stackexchange.com/questions/193066/how-to-unlock-account-for-public-key-ssh-authorization-but-not-for-password-aut
```

