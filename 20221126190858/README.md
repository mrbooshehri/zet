# Set hostname for several host with ansible

You can create a new variable for each of the servers in the inventory like 

```
[k8s_kvm_vms]
server1 new_hostname=centos1
server2 new_hostname=centos2
```

```yaml
---
- hosts: k8s_kvm_vms
  tasks:
  - name: "update hostnames"
    hostname:
      name: "{{ new_hostname }}"
```

Tags:
```
#ansible #hostname #set_hostname #sethostname
```

Related:
```
* https://stackoverflow.com/questions/58859092/how-do-i-correctly-use-the-ansible-hostname-module
* https://docs.ansible.com/ansible/latest//inventory_guide/intro_inventory.html#intro-inventory
```
