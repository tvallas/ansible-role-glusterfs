Ansible role glusterfs
=========

Installs glusterfs service and configures a volume. Note that currently this is only for small and simple setups with one brick and volume.

Requirements
------------

None

Role Variables
--------------

#### `glusterfs_brick_dir` (required)

Directory for bricks

#### `glusterfs_mount_dir` (required)
Mountpoint for glusterfs volume

#### `glusterfs_brick_name` (required)
Name for a brick

#### `glusterfs_hosts` (required)
Comma separated list of glusterfs cluster hosts

#### `glusterfs_replicas` (required)
Number of replicas

Dependencies
------------

None

Example Playbook
----------------


    - hosts: servers
      roles:
         - { role: glusterfs, tags: glusterfs}

License
-------

MIT

Author Information
------------------

Tuomas Vallaskangas tvallas@iki.fi
