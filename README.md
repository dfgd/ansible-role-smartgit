Ansible Role: SmartGit
========
[![Build Status](https://travis-ci.org/cmprescott/ansible-role-smartgit.svg?branch=master)](https://travis-ci.org/cmprescott/ansible-role-smartgit)

Installs SmartGit.

Requirements
------------

- [Darwin](http://www.syntevo.com/smartgit/documentation/6.5/show?page=introduction "Mac OS X Requirements")
  - **Mac OS X:** 10.7+ (Lion|Mountain Lion|Mavericks|Yosemite)
- [Linux](http://www.syntevo.com/smartgit/documentation/6.5/show?page=introduction "Linux Requirements are really vague")
  - Default pkg mgr is **apt** (Debian|Elementary OS|Ubuntu)

**TODO:** Generic .tar.gz for larger OS footprint

Role Variables
--------------

```yaml
# --- Remote Sources ---
smartgit_mirror: "http://www.syntevo.com/downloads/smartgit"
smartgit_version: "6_5_7"

# --- Local Destinations ---
smartgit_tmp: "/tmp"

# --- apt defaults (Debian, Elementary, Ubuntu, etc) ---
smartgit_deb_url: "{{ smartgit_mirror }}/smartgit-{{ smartgit_version }}.deb"
smartgit_tmp_deb: "{{ smartgit_tmp }}/smartgit-{{ smartgit_version }}.deb"

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
