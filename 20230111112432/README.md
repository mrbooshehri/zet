# Ansible conditional check failed 

If you faced the following message 
```
failed! => {"msg": "the conditional check 'ansible_distribution == 'centos' or ansible_distribution == 'red hat enterprise linux'' failed.
```
add the following key to your ansible playbook:
```
gather_facts: true
```

Tags:
```
#ansible #condicional #check #condicional_check
```

Related:
```
https://stackoverflow.com/questions/66496037/ansible-error-while-evaluating-conditional
```
