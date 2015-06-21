Ansible Postfix Role
====================
[![Build Status](https://semaphoreci.com/api/v1/projects/6c6ec20f-3ea1-4023-8111-468764043b33/461770/badge.svg)](https://semaphoreci.com/michaelrigart/ansible-role-postfix) [![Build Status](https://travis-ci.org/michaelrigart/ansible-role-postfix.svg?branch=master)](https://travis-ci.org/michaelrigart/ansible-role-postfix)

An ansible role for installing and configuring Postfix.

Role Variables
--------------

```yaml
postfix_apt_pkgs: list of packages to install postfix
postfix_pkg_state: indicates the package state; Allowed setting: installed, latest
postfix_service_state: indicates the service state; Allowed setting: started, stopped
postfix_service_enabled: indicates if service needs to be enabled on boot; Allowed settings: yes, no
postfix_main_config: dictionary that holds the full postfix main configuration
```

View the default vars - defaults/main.yml - for a more detailed example.

Example Playbook
-------------------------

```yaml
- hosts: servers
  roles:
     - { role: MichaelRigart.postfix, sudo: Yes }
```

License
-------

GPLv3

Author Information
------------------

Michaël Rigart <michael@netronix.be>