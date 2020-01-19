# OSM Ansible Role: MySQL

A high end ansible role to setup standalone or a cluster MySQL with best practices in terms of security and performance tunning.

## Key Features

- [X] CIS compliant
- [X] Best Practices
- [X] Database and User Management

## Requirements

No special requirement, only root access of the server is required.

## Role Variables

We have categorized variables into two part i.e. **[Manadatory]()** and **[Optional]()**

|**Variable**|**Default Value**|**Possible Values**|**Description**|
|------------|-----------------|-------------------|---------------|
|mysql_root_username| root | *Root Username* | Name of the admin user of MySQL |
|mysql_root_password| root | *Any Strong Password* | A strong password for MySQL root user |
