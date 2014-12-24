```bash
diff 1.7.2 1.8.1
7c7
< TASK: [none | touch playbook_local] ******************************************* 
---
> TASK: [none | touch {{ myvar }}] ********************************************** 
13c13
< TASK: [use_default | touch playbook_local] ************************************ 
---
> TASK: [use_default | touch {{ myvar }}] *************************************** 
19c19
< TASK: [use_var | touch playbook_local] **************************************** 
---
> TASK: [use_var | touch vars] ************************************************** 
25c25
< TASK: [use_both | touch playbook_local] *************************************** 
---
> TASK: [use_both | touch vars] ************************************************* 
```
