Raspberry Pi setup with Ansible
===

Pre-Requirements
---

### SSH service is working on Raspberry Pi

``` sh
$ sudo systemctl enable ssh
$ sudo systemctl start ssh
```

Usage
---

Prepare Inventory file ans variables file.  
See inventory/hosts.sample and group_vars/all.sample for an example file.  

``` sh
$ ansible-playbook -i inventory/hosts bootstrap.yml -k
```

After running
---

This script changes ip address and hostname.  
You need to modify inventory file to connect machines again.  
