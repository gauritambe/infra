Role Name
=========

This role sets up the infrastructure on your server. No variables are required. As a prerequisite, the docker_container collection must be installed.


Requirements
------------

Minimum server space: 20GB

Write ansible.cfg:

```bash
[defaults]
inventory=/home/devops/infrastructure/inventory
remote_user=devops
ask_pass=false
roles_path=/home/devops/infrastructure/roles
collections_paths=/home/devops/infrastructure/collections

[privilege_escalation]
become=true
become_method=sudo
become_user=root
become_ask_pass=false
```

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

ansible-galaxy collection install community.docker

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```bash
    - hosts: servers
      roles:
         - { role: username.infra, x: 42 }
```
or 
```bash
    - hosts: all
      roles:
    	 - infra
```


License
-------
License: MIT

Author Information: Gauri Tambe
------------------

Checkout my project: [Project](https://github.com/gauritambe/sap-classes)
