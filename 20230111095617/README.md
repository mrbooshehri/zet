# Ansible `password_hash`

The function just gets `string` type, so you need to parse your value
before passing it.

```yaml
- name: Add user in CentOS/RHEL hosts
  ansible.builtin.user:
    name: "{{ item.key }}"
    password: "{{ item.value | string | password_hash('sha512') }}"
    state: present  
    groups: wheel
    append: yes
  loop: "{{ none_root_users | dict2items }}"
```

Tags:
```
#ansible #password_hash #user #multiple_user
```

Related:
```
* https://www.lisenet.com/2019/ansible-generate-crypted-passwords-for-the-user-module/
```
