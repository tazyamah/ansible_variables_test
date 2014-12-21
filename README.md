output:

```bash
$ansible --version
ansible 1.8.2
  configured module search path = None
$ansible-playbook -i '127.0.0.1,' playbook.yml 

PLAY [127.0.0.1] ************************************************************** 

GATHERING FACTS *************************************************************** 
ok: [127.0.0.1]

TASK: [none | touch {{ myvar }}] ********************************************** 
changed: [127.0.0.1]

TASK: [none | touch playbook_role] ******************************************** 
changed: [127.0.0.1]

TASK: [use_default | touch {{ myvar }}] *************************************** 
changed: [127.0.0.1]

TASK: [use_default | touch playbook_role] ************************************* 
changed: [127.0.0.1]

TASK: [use_var | touch vars] ************************************************** 
changed: [127.0.0.1]

TASK: [use_var | touch playbook_role] ***************************************** 
changed: [127.0.0.1]

TASK: [use_both | touch vars] ************************************************* 
changed: [127.0.0.1]

TASK: [use_both | touch playbook_role] **************************************** 
changed: [127.0.0.1]

PLAY RECAP ******************************************************************** 
127.0.0.1                  : ok=9    changed=8    unreachable=0    failed=0
```

