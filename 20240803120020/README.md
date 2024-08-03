# How to use found objects in `find` Ansible modules

```yaml
- name: Register all files
  find:
    paths: ./files/
    patterns: '*slack*.pkg,*slack*.dmg'
    file_type: file
  register: installers
- debug:
    msg: "{{ installers.files|map(attribute='path')|map('basename')|list }}"
```


Tags:
```
#ansible #find #module #find_module
```

Related:
```
* https://stackoverflow.com/questions/73978057/ansible-use-find-module-on-registered-variable
```
