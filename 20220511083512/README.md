# Make gpg remember your passphrase

To make it remember your password, you can use ```gpg-agent``` 

Edit your ```~/.gnupg/gpg-agent.conf``` file and paste these lines

```bash
default-cache-ttl 28800
max-cache-ttl 28800
# 28800 seconds means 8 hours
```

If ```gpg-agent``` is not running you can start it with this command

```bash
gpg-agent --daemon
```

Change your key passphrase

```bash
gpg --edit-key <PASTE_YOUR_KEY_ID_HERE>
```

At the gpg prompt type:

```bash
passwd
```

Type in the current passphrase when prompted
Type in the new passphrase twice when prompted
Type:

```bash
save
```

Tags:
```
#gpg #gpg-agent
```

Related:
```
* https://gist.github.com/ankurk91/c4f0e23d76ef868b139f3c28bde057fc
```
