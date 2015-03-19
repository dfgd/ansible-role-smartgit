Ansible Role: SmartGit
========
[![Build Status](https://travis-ci.org/cmprescott/ansible-role-smartgit.svg?branch=master)](https://travis-ci.org/cmprescott/ansible-role-smartgit)


Installs SmartGit.

TODO: Consider Java & Git dependency handling.

NOTE: OS X already includes JRE and Git dependencies

Requirements
------------

Darwin (OS X): Mac OS 10.5+

Debian (Linux): all

Ubuntu (Linux): all

Role Variables
--------------

```
# --------
# Debian defaults
# --------
smartgit_debian_url: http://www.syntevo.com/downloads/smartgit/smartgit-6_5_6.deb
smartgit_debian_dir_download: /tmp

# --------
# Ubuntu defaults
# --------
smartgit_ubuntu_ppa_repo: ppa:eugenesan/ppa
```

Dependencies
------------

Darwin (OS X): Homebrew

Debian (Linux): JRE 1.7+, git

Ubuntu (Linux): JRE 1.7+, git

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
