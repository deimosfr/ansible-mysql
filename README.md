Ansible MySQL playbook
=====

This role installs and configures MySQL on a server.

Requirements
------------

This role requires Ansible 1.6 or higher and platform requirements are listed
in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about
them are as follows.

```
mysql_mysqld_bind_address: "0.0.0.0"
mysql_root_username: root
mysql_root_password: password
```
All variables can be found in the defaults folder.

Examples
========

To setup a MySQL instance, it's simple:

```
# Roles
- name: sql
  hosts: sql
  user: root
  roles:
    - mysql
  vars_files:
    - group_vars/mysql.yml

```

Dependencies
------------

None

License
-------

GPL

Author Information
------------------

Pierre Mavro / deimosfr


