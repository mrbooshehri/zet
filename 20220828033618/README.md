# Change the pushed commit message

## Last git commit

```bash
git commit --amend -m "New message"
git push --force repository-name branch-name
```
## Older or multiple messages

```bash
git rebase -i HEAD~3
pick e499d89 Delete CNAME
pick 0c39034 Better README
pick f7fde4a Change the commit message but push the same commit.
git push --force
```

Tags:
```
#git #commit_message #change_commit_message
```

Related:
```
* https://medium.com/@_oleksii_/how-to-change-a-commit-message-in-git-after-push-32d1fbd6fc3b
```
