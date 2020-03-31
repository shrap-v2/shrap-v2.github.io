# Sample ansible.cfg

```bash
[defaults]
host_key_checking = False
deprecation_warnings = False
retry_files_enabled = False
# strategy_plugins = /etc/ansible/plugins/mitogen-0.2.9/ansible_mitogen/plugins/strategy
# strategy = mitogen_linear
callback_whitelist = profile_tasks #Provides timestamps (See Performance Tuning Note)

[inventory]
[privilege_escalation]
[paramiko_connection]
[ssh_connection]
[persistent_connection]
[accelerate]
[selinux]
[colors]
[diff]
```
