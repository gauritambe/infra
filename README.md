Role Name
=========

This role sets up the infrastructure on your server. No variables are required. As a prerequisite, the docker_container collection must be installed.


Requirements
------------

Minimum server space: 20GB


Dependencies
------------

ansible-galaxy collection install community.docker

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - infra

License: MIT
-------

BSD

Author Information: Gauri Tambe
------------------

Checkout my project: [Project](https://github.com/gauritambe/sap-classes)
