# XFCE auto login

Add the following configs under `[Seat:*]` in `/etc/lightdm/lightdm.conf`

```bash
[Seat:*]
...
autologin-session=xubuntu
autologin-user=YourDesiredAutoLoginUserName
autologin-user-timeout=0
...
```

Tags:
```
#linux #xfce #desktop #auto #login #autologin #auto_login
```

Related
```
* https://askubuntu.com/questions/530072/how-to-auto-login-in-xubuntu-or-ubuntu-server-with-xfce
```
