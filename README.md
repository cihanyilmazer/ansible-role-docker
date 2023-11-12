Role Name
=========

This role installs and configures docker, containerd and docker-compose on Ubuntu 20.04 and later.

Requirements
------------

Operating System: Ubuntu 20.04 or later

Role Variables
--------------

#Optional
```
# docker_user: root
# docker_address_pool_base: 172.20.0.0/16
# docker_address_pool_size: 24
```

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Install
```
ansible-galaxy install cihanyilmazer.docker
```

    - hosts: servers
      roles:
         - cihanyilmazer.docker

Run with Custom Tags (at least one tag must be provided)
- docker
- docker-install
- docker-configure

```
ansible-playbook -i hosts playbook.yml --tags docker --limit servers

License
-------

MIT

Author Information
------------------

Cihan Yilmazer<br />
https://www.cihanyilmazer.com<br />
https://www.github.com/cihanyilmazer<br />
