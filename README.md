# Install PostgreSQL-12 on Centos 8 using Ansible Role

## Features:

1. Supported distributions: 8 version of Redhat, CentOS, Scientific Linux.
2. Oracle Linux also supported but uses RHEL repositories.
3. supported PostgreSQL version: 12
4. allows specify users and databases which would be created after install.
5. Jinja2 template is used for postgresql.conf 

## How-to use:

Download the repo with git clone;
Change hosts: in playbook.yml according to your host groups
```
---
- hosts: postgresql
    roles:
    - PostgreSQLRole
    become: yes
```
Start ansible-playbook with playbook.yml and add -i if you want to use inventory file.

```
ansible-playbook playbook.yml -vv
```


Author Information
------------------

[Nareshkar Pakanati](https://github.com/DevOpsThinkk)  
