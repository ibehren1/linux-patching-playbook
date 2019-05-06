# Linux Patching Playbook

Ansible playbook for patching Ubuntu/Debian/RHEL/CentOS/Amazon Linux hosts.

### How to run:
```
ansible-playbook main.yml \
  --private-key <path to key> \
  -u <username> \
  -i hosts \
  -l <host-group> \
  [--extra-vars reboot_ok=true]
```

The playbook does not reboot hosts by default.  
To reboot hosts when necessary, override the reboot_ok variable from the command line as shown above.  

---
Author:   Isaac Behrens  
Date:     February 7, 2019  
