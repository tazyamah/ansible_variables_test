output:

```bash
$ansible --version
ansible 1.8.2
  configured module search path = None
$vagrant provision
==> default: Running provisioner: ansible...

PLAY [vagrant] **************************************************************** 

GATHERING FACTS *************************************************************** 
ok: [192.168.50.50]

TASK: [none | touch {{ myvar }}] ********************************************** 
changed: [192.168.50.50]

TASK: [none | touch playbook_role] ******************************************** 
changed: [192.168.50.50]

TASK: [use_default | touch {{ myvar }}] *************************************** 
changed: [192.168.50.50]

TASK: [use_default | touch playbook_role] ************************************* 
changed: [192.168.50.50]

TASK: [use_var | touch vars] ************************************************** 
changed: [192.168.50.50]

TASK: [use_var | touch playbook_role] ***************************************** 
changed: [192.168.50.50]

TASK: [use_both | touch vars] ************************************************* 
changed: [192.168.50.50]

TASK: [use_both | touch playbook_role] **************************************** 
changed: [192.168.50.50]

PLAY RECAP ******************************************************************** 
192.168.50.50              : ok=9    changed=8    unreachable=0    failed=0   
```

