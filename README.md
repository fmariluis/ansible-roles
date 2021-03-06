# Ansible roles [![Build Status](https://travis-ci.org/MSA-Argentina/ansible-roles.svg?branch=master)](https://travis-ci.org/MSA-Argentina/ansible-roles)

Some useful roles to speed up deployments with Ansible. Requires Ansible 2.0+ and Ubuntu 16.04. Most roles also work in FreeBSD (tested in 10.3+)

## How to use
* Clone this repo
* Modify `ansible.cfg` (usually `/etc/ansible/ansible.cfg`) and include this line:
```
roles_path = /path/to/cloned_repo
```
* Finally, use any of these roles in your playbooks:
```
---
- hosts: all
  roles:
    - server-bootstrap
    - postgresql
    - nginx
...
```

# Credits

* PostgreSQL role from https://github.com/ansibles/postgresql
* Memcached role from https://github.com/bennojoy/memcached
* ElasticSearch role from https://github.com/deimosfr/ansible-elasticsearch
* Java role from https://github.com/vrischmann/ansible-role-java
* Jenkins role from https://github.com/binarytemple/ansible-role-jenkins.git
