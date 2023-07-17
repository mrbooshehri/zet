# Adding line with special character in Ansible

Instead of using the following:
```yaml
  tasks:
    - name: Add line to .bashrc
      ansible.builtin.lineinfile:
        path: ~/.bashrc
        line: 'export PROMPT_COMMAND=\'history -a >(tee -ia ~/.bash_history | logger -t "LnxCmd: Date: $(date "+%Y-%m-%d %H:%M:%S") User: [ $USER ] Shell PID: [$$] command")\''
        insertafter: EOF
```

Do this style:
```yaml
  tasks:
    - name: Add line to .bashrc
      ansible.builtin.lineinfile:
        path: ~/.bashrc
        line: |
				  export PROMPT_COMMAND=\'history -a >(tee -ia ~/.bash_history | logger -t "LnxCmd: Date: $(date "+%Y-%m-%d %H:%M:%S") User: [ $USER ] Shell PID: [$$] command")'
        insertafter: EOF
```

Tags:
```
#Ansible #lineinfile #special #character #special_character
```

Related:
```
* Just me :)
```
