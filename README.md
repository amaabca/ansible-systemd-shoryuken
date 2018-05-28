Role Name
=========

Adds systemd configuration for a [Shoryuken](https://github.com/phstc/shoryuken) worker process deployed with Capistrano 3 on Ubuntu 16.04.

Requirements
------------

A functioning Rails deployment using Capistrano 3 on Ubuntu 16.04 is required to use this role.

Role Variables
--------------

**ansible_systemd_shoryuken_user**: The owner of the Shoryuken process.
**ansible_systemd_shoryuken_app_path**: The full path to the Capistrano 3 deployment directory.


Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - role: amaabca.ansible-systemd-shoryuken
       ansible_systemd_shoryuken_user: appserver
       ansible_systemd_shoryuken_app_path: /srv/myapp
```

License
-------

MIT

Author Information
------------------

https://github.com/amaabca/ansible-systemd-shoryuken
