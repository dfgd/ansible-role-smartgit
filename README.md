Ansible Role: SmartGit
========
[![Build Status](https://travis-ci.org/cmprescott/ansible-role-smartgit.svg?branch=master)](https://travis-ci.org/cmprescott/ansible-role-smartgit)


Installs SmartGit.

Requirements
------------

Debian (Linux): None

Darwin (OS X): Homebrew

Role Variables
--------------

```
# --------
# Debian based default repo
# --------
smartgit_debian_ppa_repo: ppa:eugenesan/ppa
```

Dependencies
------------

Debian (Linux): None

Darwin (OS X): If you don't have homebrew; use an Ansible role like geerlingguy.homebrew to install it

Example Playbook
-------------------------

    - hosts: development
      roles:
        - { role: ansible-role-smartgit, sudo: Yes }

License
-------

BSD

Author Information
------------------

Prescott Chris
