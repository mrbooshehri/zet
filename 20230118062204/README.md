# Caching maven dependences gitlab
```yaml
cache:
  key: ${CI_COMMIT_REF_SLUG}
  paths:
    - m2/repository
```

Tags:
```
#gitlab #maven #cache
```

Related:
```
https://medium.com/devops-with-valentine/caching-maven-dependencies-in-a-gitlab-ci-pipeline-c50017085a2
```
