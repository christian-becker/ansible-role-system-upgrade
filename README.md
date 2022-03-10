system_upgrade
==============

This ansible role upgrades all packages on linux and windows systems.
In default configuration all packages will be upgraded to the latest version available. A windows system will automatically reboot if it is required and continue to install updates after the reboot (if it's not disabled in ansible variable).


Requirements
------------

This role has no special requirements.


Role Variables
--------------

Here is a list of variables defined in **defaults/main.yml**: 

```
# reboot the windows system automatically
system_upgrade_windows_reboot: 'yes'
```


Dependencies
------------

This role has no dependencies.


Example Playbook
----------------

This role can be used e.g. with the following playbook:
```
---
- name: upgrade all packages on system
  hosts: server
  remote_user: root
  roles:
    - christian_becker.system_upgrade
```


License
-------

MIT


Author Information
------------------

* **Christian Becker** - [christian-becker](https://github.com/christian-becker)  

