Ansible Role: SmartGit
========

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
         role: smartgit

License
-------

BSD

Author Information
------------------

Prescott Chris
