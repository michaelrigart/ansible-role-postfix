Ansible Postfix Role
====================

An ansible role for installing and configuring Postfix.

Role Variables
--------------

postfix_apt_pkgs: list of packages to install postfix
postfix_pkg_state: indicates the package state; Allowed setting: installed, latest
postfix_service_state: indicates the service state; Allowed setting: started, stopped
postfix_service_enabled: indicates if service needs to be enabled on boot; Allowed settings: yes, no
postfix_main_config: dictionary that holds the full postfix main configuration

View the default vars - defaults/main.yml - for a more detailed example.

Example Playbook
-------------------------

    - hosts: servers
      roles:
         - { role: MichaelRigart.postfix }

License
-------

GPLv3

Author Information
------------------

Michaël Rigart <michael@netronix.be>