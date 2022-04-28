# Apache Server Tokens

```
ServerTokens Major|Minor|Min|Prod|OS|Full
```

1. ServerTokens Full
the server will send the full information to the remote host.
```
Server: Apache/2.0.41 (Unix) PHP/4.2.2 MyMod/1.2
```

1. ServerTokens OS
The server will send the Web server version and the operating system
version.
```
Server: Apache/2.0.41 (Unix)
```

1. ServerTokens Min
the server will send the Web server’s full version number like
Apache2.0.41.
```
Apache/2.0.41
``` 
**This is also a security issue as the remote user will try to hack the server
with security holes in Apache2.0.41 versions.**

1. ServerTokens Minor
The server will send the Web server’s minor version number like Apache
version2.0.
```
Apache/2.0
```
**This is also a security issue as the remote user will try to hack the server
with security holes in Apache 2.0 versions.**

1. ServerTokens Major
 the server will send the Web server’s minor version number like Apache
 version2.
```
 Apache/2
```
**This is also a security issue as the remote user will try to hack the server with
 security holes in Apache 2 version.**

 1. ServerTokens Prod
 The server will send the Web server’s name alone, which is recommended
 as the hacker will not have a clue of which version of Apache is
 running in the server and also which operating system is used. The
 information sent will be “Server: Apache”.

 Tags:
 ```
 #Linux #Apache #ServerToken #security
 ```

 Related:
 ```
 * <https://actsupport.com/six-basic-options-configure-apache-token/>
 ```
