mysql-server
============

An ansible role for the installation of MySQL on Ubuntu(14,16) and CemtOS(6,7).

Requirements
------------

None

Role Variables
--------------

```
mysql_root_password: "root"
mysql_user_name: "opstree"
mysql_user_password: "opstree"
mysql_database_name: "opstree"
```

Dependencies
------------

None

Example Playbook
----------------

A playbook to use the role.

```
---
  - hosts: hostgroup/host
    become: true
    roles: 
      - mysql-server
```

License
-------

BSD

Author Information
------------------

```
Name: Anupam Yaadav
Email: anupam.singh.yadav@opstree.com
```
