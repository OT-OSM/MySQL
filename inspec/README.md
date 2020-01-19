## CIS Practices to be Fixed

```
  ×  4.4: Ensure 'local_infile' Is Disabled (Scored)
     ×  The MySQL local_infile setting should cmp == 0
     
     expected: 0
          got: ""
     
     (compared using `cmp` matcher)

  ×  3.6: Ensure 'general_log_file' Has Appropriate Permissions and Ownership (Scored) (4 failed)
     ×  Directory [] should exist
     expected Directory [] to exist
     ×  Directory [] owner should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] group should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] mode should be <= 432
     expected: <= 432
          got:    nil
  ✔  7.3: Ensure Passwords Are Not Stored in the Global Configuration (Scored)
     ✔  MySQL Configuration client.password should be nil
  ×  3.2: Ensure 'log_bin_basename' Files Have Appropriate Permissions and Ownership (Scored) (4 failed)
     ×  Directory [] should exist
     expected Directory [] to exist
     ×  Directory [] owner should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] group should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] mode should be <= 432
     expected: <= 432
          got:    nil
  ×  3.7: Ensure SSL Key Files Have Appropriate Permissions and Ownership (Scored) (4 failed)
     ×  Directory [] should exist
     expected Directory [] to exist
     ×  Directory [] owner should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] group should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] mode should be <= 256
     expected: <= 256
          got:    nil
  ↺  2.4: Do Not Use Default or Shared Cryptographic Material (Not Scored)
     ↺  A manual review is required to ensure the default or shared cryptographic material is not being used
  ↺  5.4: Ensure 'super_priv' Is Not Set to 'Y' for Non-Administrative Users (Scored)
     ↺  There are no mysql users with super_priv allowed, therefore this control is not applicable
  ×  3.9: Ensure 'audit_log_file' has Appropriate Permissions and Ownership (Scored) (4 failed)
     ×  Directory [] should exist
     expected Directory [] to exist
     ×  Directory [] owner should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] group should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] mode should be <= 432
     expected: <= 432
          got:    nil
  ×  6.1: Ensure 'log_error' Is Not Empty (Scored)
     ×  The MySQL log_error should not be empty
     expected `[].empty?` to return false, got true
  ×  3.4: Ensure 'slow_query_log' Has Appropriate Permissions and Ownership (Scored) (4 failed)
     ×  Directory [] should exist
     expected Directory [] to exist
     ×  Directory [] owner should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] group should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] mode should be <= 432
     expected: <= 432
          got:    nil
  ↺  2.3: Do Not Reuse User Accounts (Not Scored)
     ↺  There are no mysql database users, therefore this control is not applicable
  ×  4.6: Ensure '--skip-symbolic-links' Is Enabled (Scored)
     ×  MySQL Configuration skip_symbolic_links should cmp == "YES"
     
     expected: "YES"
          got: nil
     
     (compared using `cmp` matcher)

  ×  6.12: Make sure the audit plugin can't be unloaded (Scored) (2 failed)
     ×  The MySQL audit plugin should cmp == "FORCE_PLUS_PERMANENT"
     
     expected: "FORCE_PLUS_PERMANENT"
          got: ""
     
     (compared using `cmp` matcher)

     ×  MySQL Configuration mysqld.audit_log should cmp == "FORCE_PLUS_PERMANENT"
     
     expected: "FORCE_PLUS_PERMANENT"
          got: nil
     
     (compared using `cmp` matcher)

  ×  1.3: Disable MySQL Command History (Scored)
     ×  The MySql history file: ["/root/.mysql_history"] link_path should eq "/dev/null"
     
     expected: "/dev/null"
          got: nil
     
     (compared using ==)

  ×  7.2: Ensure 'secure_auth' is set to 'ON' (Scored)
     ×  The MySQL secure_auth should cmp == 1
     
     expected: 1
          got: ""
     
     (compared using `cmp` matcher)

  ×  6.3: Ensure 'log_warnings' Is Set to '2' (Scored)
     ×  The MySQL log_warnings should cmp == 2
     
     expected: 2
          got: ""
     
     (compared using `cmp` matcher)

  ×  3.3: Ensure 'log_error' Has Appropriate Permissions and Ownership (Scored) (4 failed)
     ×  Directory [] should exist
     expected Directory [] to exist
     ×  Directory [] owner should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] group should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] mode should be <= 432
     expected: <= 432
          got:    nil
  ↺  8.2: Ensure 'ssl_type' Is Set to 'ANY', 'X509', or 'SPECIFIED' for All Remote Users (Scored)
     ↺  There are no mysql remote users, therefore this control is not applicable
  ✔  9.5: Ensure No Replication Users Have Wildcard Hostnames (Scored)
     ✔  The replication users with the super_priv not set to Y should be empty
  ↺  5.5:  Ensure 'shutdown_priv' Is Not Set to 'Y' for Non-Administrative Users (Scored)
     ↺  There are no mysql users with shutdown_priv allowed, therefore this control is not applicable
  ↺  5.6: Ensure 'create_user_priv' Is Not Set to 'Y' for Non-Administrative Users (Scored)
     ↺  There are no mysql users with create_user_priv allowed, therefore this control is not applicable
  ×  4.8: Ensure 'secure_file_priv' Is Not Empty (Scored)
     ×  The secure_file_priv variable should not be empty
     expected `"".empty?` to return false, got true
  ×  6.11: Set audit_log_strategy to SYNCHRONOUS or SEMISYNCRONOUS (Scored) (2 failed)
     ×  The MySQL audit_log_strategy variable should cmp == "SYNCHRONOUS"
     
     expected: "SYNCHRONOUS"
          got: ""
     
     (compared using `cmp` matcher)

     ×  The MySQL audit_log_strategy variable should cmp == "SEMISYNCHRONOUS"
     
     expected: "SEMISYNCHRONOUS"
          got: ""
     
     (compared using `cmp` matcher)

  ✔  4.3: Ensure 'allow-suspicious-udfs' Is Set to 'FALSE' (Scored)
     ✔  MySQL Configuration allow-suspicious-udfs should be nil
     ✔  Command: `ps aux | grep mysql` stdout should not match "allow-suspicious-udfs"
  ✔  7.1: Ensure 'old_passwords' Is Not Set to '1' (Scored)
     ✔  The MySQL old_passwords should not cmp == 1
  ×  9.2: Ensure 'MASTER_SSL_VERIFY_SERVER_CERT' Is Set to 'YES' or '1' (Scored)
     ×  The MASTER_SSL_VERIFY_SERVER_CERT should cmp == 1
     
     expected: 1
          got: ""
     
     (compared using `cmp` matcher)

  ↺  5.7: Ensure 'grant_priv' Is Not Set to 'Y' for Non-Administrative Users (Scored)
     ↺  There are no mysql users configured with grant_priv access, therefore this control is not applicable
  ↺  9.1: Ensure Replication Traffic Is Secured (Not Scored)
     ↺  A manual review is required to ensure the replication traffic is secured
  ×  6.7: Ensure audit_log_include_accounts is set to NULL (Scored)
     ×  The MySQL audit_log_include_accounts should cmp == "NULL"
     
     expected: "NULL"
          got: ""
     
     (compared using `cmp` matcher)

  ×  7.6: Ensure Password Policy Is in Place (Scored) (8 failed)
     ×  The MySQL validate_password_length variable should cmp >= 14
     
     expected it to be >= 14
          got: ""
     
     (compared using `cmp` matcher)

     ×  The MySQL validate_password_mixed_case_count variable should cmp >= 1
     
     expected it to be >= 1
          got: ""
     
     (compared using `cmp` matcher)

     ×  The MySQL validate_password_number_count variable should cmp >= 1
     
     expected it to be >= 1
          got: ""
     
     (compared using `cmp` matcher)

     ×  The MySQL validate_password_special_char_count variable should cmp >= 1
     
     expected it to be >= 1
          got: ""
     
     (compared using `cmp` matcher)

     ×  The MySQL validate_password_policy variable should cmp == "MEDIUM"
     
     expected: "MEDIUM"
          got: ""
     
     (compared using `cmp` matcher)

     ×  The MySQL validate_password_policy variable should cmp == "STRONG"
     
     expected: "STRONG"
          got: ""
     
     (compared using `cmp` matcher)

     ×  MySQL Configuration plugin-load should cmp == "validate_password.so"
     
     expected: "validate_password.so"
          got: nil
     
     (compared using `cmp` matcher)

     ×  MySQL Configuration validate-password should cmp == "FORCE_PLUS_PERMANENT"
     
     expected: "FORCE_PLUS_PERMANENT"
          got: nil
     
     (compared using `cmp` matcher)

     ✔  The MySQL users with their password identical to their username should be empty
  ✔  9.4: Ensure 'super_priv' Is Not Set to 'Y' for Replication Users (Scored)
     ✔  The replication users with the super_priv not set to Y should be empty
  ×  9.3: Ensure 'master_info_repository' Is Set to 'TABLE' (Scored)
     ×  The master_info_repository should cmp == "TABLE"
     
     expected: "TABLE"
          got: ""
     
     (compared using `cmp` matcher)

  ↺  5.8: Ensure 'repl_slave_priv' Is Not Set to 'Y' for Non-Slave Users (Scored)
     ↺  There are no mysql users with repl_slave_priv allowed, therefore this control is not applicable
  ✔  1.5: Disable Interactive Login (Scored)
     ✔  /etc/passwd with user == "mysql" shells should cmp == "/bin/false"
  ↺  5.2: Ensure 'file_priv' Is Not Set to 'Y' for Non-Administrative Users (Scored)
     ↺  There are no mysql users with file_priv allowed, therefore this control is not applicable
  ×  4.1: 4.1 Ensure Latest Security Patches Are Applied (Not Scored)
     ×  The mysql version installed should cmp >= "5.7.24-enterprise-commercial-advanced"
     
     expected it to be >= "5.7.24-enterprise-commercial-advanced"
          got: ""
     
     (compared using `cmp` matcher)

  ×  8.1: Ensure 'have_ssl' Is Set to 'YES' (Scored)
     ×  The MySQL have_ssl variable should cmp == "YES"
     
     expected: "YES"
          got: ""
     
     (compared using `cmp` matcher)

  ×  7.4: Ensure 'sql_mode' Contains 'NO_AUTO_CREATE_USER' (Scored) (2 failed)
     ×  The MySQL global sql mode should include "NO_AUTO_CREATE_USER"
     expected "" to include "NO_AUTO_CREATE_USER"
     ×  The MySQL session sql mode should include "NO_AUTO_CREATE_USER"
     expected "" to include "NO_AUTO_CREATE_USER"
  ✔  1.2: Use Dedicated Least Privileged Account for MySQL Daemon/Service (Scored)
     ✔  The user runnning the MySQL Daemon/Service should cmp == "mysql"
  ×  6.4: Ensure 'log-raw' Is Set to 'OFF' (Scored)
     ×  MySQL Configuration log-raw should cmp == "OFF"
     
     expected: "OFF"
          got: nil
     
     (compared using `cmp` matcher)

  ↺  5.1: Ensure Only Administrative Users Have Full Database Access (Scored)
     ↺  There are no mysql users configured with full database access, therefore this control is not applicable
  ✔  6.2: Ensure Log Files Are Stored on a Non-System Partition (Scored)
     ✔  The mysql log files partition installed on should not include "/"
     ✔  The mysql log files partition installed on should not include "/var"
     ✔  The mysql log files partition installed on should not include "/usr"
  ×  6.10: Ensure audit_log_statement_policy is set to ALL (Scored)
     ×  The MySQL log_error should not be empty
     expected `[].empty?` to return false, got true
  ✔  1.1: 1.1 Place Databases on Non-System Partitions (Scored)
     ✔  The mysql data directory partition installed on should not include "/"
     ✔  The mysql data directory partition installed on should not include "/var"
     ✔  The mysql data directory partition installed on should not include "/usr"
  ×  6.9: Ensure audit_log_policy is set to log logins and connections (Scored)
     ×  The MySQL audit_log_policy should cmp == "ALL"
     
     expected: "ALL"
          got: ""
     
     (compared using `cmp` matcher)

  ×  3.8: Ensure Plugin Directory Has Appropriate Permissions and Ownership (Scored) (4 failed)
     ×  Directory [] should exist
     expected Directory [] to exist
     ×  Directory [] owner should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] group should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] mode should be <= 509
     expected: <= 509
          got:    nil
  ✔  1.4: Verify that 'MYSQL_PWD' Is Not Set (Scored)
     ✔  The MYSQL_PWD environment variable should eq ""
  ↺  5.3: Ensure 'process_priv' Is Not Set to 'Y' for Non-Administrative Users (Scored)
     ↺  There are no mysql users with process_priv allowed, therefore this control is not applicable
  ✔  7.7: Ensure No Users Have Wildcard Hostnames (Scored)
     ✔  The MySQL users that have Wildcard Hostnames should be empty
  ×  3.5: Ensure 'relay_log_basename' Files Have Appropriate Permissions and Ownership (Scored) (4 failed)
     ×  Directory [] should exist
     expected Directory [] to exist
     ×  Directory [] owner should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] group should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] mode should be <= 432
     expected: <= 432
          got:    nil
  ↺  5.9: Ensure DML/DDL Grants Are Limited to Specific Databases and Users (Scored)
     ↺  There are no mysql users allowed to modify or create data structures, therefore this control is not applicable
  ×  2.2:  Do Not Specify Passwords in Command Line (Not Scored)
     ×  The linux bash history file content should not include "test1234"
     expected nil not to include "test1234", but it does not respond to `include?`
  ✔  7.8: Ensure No Anonymous Accounts Exist (Scored)
     ✔  The MySQL anonymous accounts that exist should be empty
  ×  6.8: Ensure audit_log_policy is set to log logins (Scored) (2 failed)
     ×  The MySQL audit_log_policy should cmp == "ALL"
     
     expected: "ALL"
          got: ""
     
     (compared using `cmp` matcher)

     ×  The MySQL audit_log_policy 
     undefined local variable or method `audit_log_policyy' for #<RSpec::ExampleGroups::TheMySQLAuditLogPolicy_3:0x000055f3a6a405c0>
     
     undefined local variable or method `audit_log_policyy' for #<RSpec::ExampleGroups::TheMySQLAuditLogPolicy_3:0x000055f3a851c510>
  ×  3.1: Ensure 'datadir' Has Appropriate Permissions and Ownership (Scored) (4 failed)
     ×  Directory [] should exist
     expected Directory [] to exist
     ×  Directory [] owner should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] group should eq "mysql"
     
     expected: "mysql"
          got: nil
     
     (compared using ==)

     ×  Directory [] mode should be <= 448
     expected: <= 448
          got:    nil
  ✔  4.2: Ensure the 'test' Database Is Not Installed (Scored)
     ✔  The check wether the test database is installed should be empty
  ×  4.9: Ensure 'sql_mode' Contains 'STRICT_ALL_TABLES' (Scored)
     ×  The sql_mode should include "STRICT_ALL_TABLES"
     expected "" to include "STRICT_ALL_TABLES"
  ×  6.6: Ensure audit_log_exclude_accounts is set to NULL (Scored)
     ×  The MySQL audit_log_exclude_accounts should cmp == "NULL"
     
     expected: "NULL"
          got: ""
     
     (compared using `cmp` matcher)

  ×  6.5: Ensure audit_log_connection_policy is not set to 'NONE' (Scored) (2 failed)
     ×  The MySQL audit_log_connection_policy should cmp == "ALL"
     
     expected: "ALL"
          got: ""
     
     (compared using `cmp` matcher)

     ×  The MySQL audit_log_connection_policy should cmp == "ERRORS"
     
     expected: "ERRORS"
          got: ""
     
     (compared using `cmp` matcher)

  ✔  7.5: Ensure Passwords Are Set for All MySQL Accounts (Scored)
     ✔  The MySQL users with blank passwords should be empty
  ×  4.5: Ensure 'mysqld' Is Not Started with '--skip-grant-tables' (Scored)
     ×  MySQL Configuration skip-grant-tables should cmp == "FALSE"
     
     expected: "FALSE"
          got: nil
     
     (compared using `cmp` matcher)

  ↺  2.1: Dedicate Machine Running MySQL (Not Scored)
     ↺  A manual review is required to verfify a dedicated machine is running MySQL
  ✔  4.7: Ensure the 'daemon_memcached' Plugin Is Disabled (Scored)
     ✔  The daemon_memcached plugins installed should be empty


Profile Summary: 15 successful controls, 34 control failures, 14 controls skipped
Test Summary: 21 successful, 73 failures, 14 skipped
```