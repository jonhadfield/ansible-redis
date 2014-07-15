redis
========

Ansible role which installs and configures redis.

Requirements
------------

Tested on Anbsible 1.6

Role Variables
--------------
    redis_online_install: true          # Whether or not to perform an online installation by downloading the installer and plugins
    redis_installer_path: /var/red      # Where to find the installer for an offline installation
    redis_version: 2.8.8                # The version of redis to install
    redis_base_install_dir: /apps       # Where redis will be installed
    redis_base_logs_dir: /logs          # Where redis' log directory will be created
    redis_base_data_dir: /data          # Where redis' data directory will be created
    redis_maxmemory:                    # Maximum amount of data redis will store in memory
    redis_maxmemory_policy:             # The policy to follow when maxmemory is reached 

Dependencies
------------

None

Example Playbook
-------------------------

    - hosts: all
      sudo: yes
      roles:
         - redis

License
-------

MIT

Author Information
------------------

Jon Hadfield
