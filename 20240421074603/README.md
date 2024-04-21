# Hot to re-enable upload plugin in Jira

Open `setenv.sh` file an add the `-Dupm.plugin.upload.enabled=true`
option

1. Open the file 
```bash
vim /PATH/TO/JIRA/HOME/bin/setenv.sh
```
2. Add `-Dupm.plugin.upload.enabled=true` option to
	 `JVM_SUPPORT_RECOMMENDED_ARGS` variable

```bash
...

JVM_SUPPORT_RECOMMENDED_ARGS="-Dupm.plugin.upload.enabled=true"

...

```
3. Restart Jira service

Tags:
```
#jira #atlassian #upload #plugin
```

Related:
```
* https://confluence.atlassian.com/jirakb/how-to-re-enable-plugin-upload-1364557898.html
```
