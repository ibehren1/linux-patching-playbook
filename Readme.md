# Ubuntu Patching Playbook

Ansible playbook for patching Ubuntu hosts.

### How to run:
```
ansible-playbook -b -u <username> --private-key <path to key> -i hosts -l <host-group> main.yml [--extra-vars reboot_ok=true]
```

The playbook does not reboot hosts by default.  
To reboot hosts when necessary, override the reboot_ok variable from the command line as shown above.  

---
Author:   Isaac Behrens  
Date:     February 7, 2019  
