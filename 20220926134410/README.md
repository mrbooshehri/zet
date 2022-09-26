# User wildcard in CI/CD yaml

If you want to user wild card in CI/CD yaml, like gitlab don't use any
special character, like:

```yml
...
sshpass -p "$SSH_PASS" scp -o StrictHostKeyChecking=no -r target/*.jar root@$MOI_ALTERNATIVE:/mnt/arbaeen/arbaeen.jar
...
```

Tags:
```
#cicd #gitlab #wildcard
```

Related:
```
* Sana Moradi :)
```
