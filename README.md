Ansible Role: SmartGit
========
[![Build Status](https://travis-ci.org/cmprescott/ansible-role-smartgit.svg?branch=master)](https://travis-ci.org/cmprescott/ansible-role-smartgit)

Installs SmartGit.

Requirements
------------

- [Darwin](http://www.syntevo.com/smartgit/documentation/6.5/show?page=introduction "Mac OS X Requirements")
  - **Mac OS X:** 10.7+ (Lion|Mountain Lion|Mavericks|Yosemite)
- [Linux](http://www.syntevo.com/smartgit/documentation/6.5/show?page=introduction "Linux Requirements are really vague")
  - **Debian:** all
  - **Ubuntu:** all

**TODO:** Generic .tar.gz for larger OS footprint

Role Variables
--------------

OS-level details should have you covered, but just in case

```yaml
smartgit_pkg_install_using: ( Debian_dpkg | MacOSX_homebrew | Ubuntu_apt )
smartgit_pkg_url: ( 'ppa:eugenesan/ppa' | 'http://www.syntevo.com/downloads/smartgit/smartgit-6_5_6.deb' )
smartgit_dir_download: /tmp 
```

Dependencies
------------

- **Darwin (Mac OS X)**: homebrew
- **Linux**: JRE 1.7+, git

**TODO:** Java & Git dependency handling.

**NOTE TO SELF:** OS X already includes JRE and Git dependencies

Example Playbook
-------------------------

```yaml
- hosts: development
  roles:
    - role: ansible-role-smartgit
```

License
-------

BSD

Author Information
------------------

Prescott Chris
