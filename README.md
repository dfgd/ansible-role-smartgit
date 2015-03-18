Ansible Role: SmartGit
========
[![Build Status](https://travis-ci.org/cmprescott/ansible-role-smartgit.svg?branch=master)](https://travis-ci.org/cmprescott/ansible-role-smartgit)


Installs SmartGit.

Requirements
------------

Darwin (OS X): Homebrew

Ubuntu (Linux): None

Role Variables
--------------

```
# --------
# Debian based default repo
# --------
smartgit_ubuntu_ppa_repo: ppa:eugenesan/ppa
```

Dependencies
------------

Darwin (OS X): If you don't have homebrew; use an Ansible role like geerlingguy.homebrew to install it

Ubuntu (Linux): None

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
