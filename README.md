# OSM: MySQL

A high end ansible role to setup standalone or a cluster MySQL with best practices in terms of security and performance tunning.

## Key Features

- [X] CIS compliant
- [X] Best Practices
- [X] Database and User Management

## Requirements

No special requirement, only root access of the server is required.

## Role Variables

We have categorized variables into two part i.e. **[Manadatory]()** and **[Optional]()**

#### Mandatory Variables

|**Variable**|**Default Value**|**Possible Values**|**Description**|
|------------|-----------------|-------------------|---------------|
|mysql_root_username| `root` | *Root Username* | Name of the admin user of MySQL |
|mysql_root_password| `root` | *Any Strong Password* | A strong password for MySQL root user |
|mysql_replication_user.user | `slave` | *Any Username* | Name of the slave user |
|mysql_replication_user.password | `slave` | *Any Strong Password* | A strong password for MySQL Slave |
|mysql_install_packages | `true` | true or false | Whether you want to install MySQL packages. Set the value false if you need only configuration part |
|replication | `true` | true or false | If you don't want to setup slave, set the value false |
|users_creation | `true` | true or false | Whether you want to include tasks for user creation or not |
|database_creation | `true` | true or false | Whether you want to include tasks for database creation or not |

#### Optional Variables

|**Variable**|**Default Value**|**Possible Values**|**Description**|
|------------|-----------------|-------------------|---------------|
|mysql_config_file| `/etc/mysql/my.cnf` | *Any Linux Path* | Configuration file location of MySQL |
|mysql_slow_query_log_file | `/var/log/mysql/mysql-slow.log` | *Any Linux Path* | Log file location of MySQL slow query |
|mysql_log_error | `/var/log/mysql/mysql.err` | *Any Linux Path* | Log file location of MySQL errors |
|mysql_max_binlog_size | `100M` | *Size in MB* | Maximum size of bin log files in MySQL |
|mysql_binlog_format | `MIXED` | ROW or COLOUMN or MIXED | Binlog format of MySQL |
