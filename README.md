# ansible_lihas_journald
Install/activate systemd-journald and possibly deactivate other syslog daemons

## Requirements

To run solo:
```
ansible-playbook -i localhost, journald.yml
```

## Dependencies

## Example Playbook

```
---
- name: Handle systemd-journald
  hosts: '*'
  roles:
    - lihas_journald
...
```
## Tags

## Variables
```
lihas_systemd_journald_max_use: maximum used space for journals, default 2G
lihas_syslog_remove: remove other syslog daemons, default false
lihas_syslog_remove_logs: remove old log files, default false
```

## Variables example
```
```
