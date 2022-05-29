ansible_nfs_client
=========

Ansible role to setup nfs client service and mount nfs share

Requirements
------------

You must have an nfs server already set up. This role is just for connecting clients.

Role Variables
--------------

| Variable            | Description                    | Example                    |
|---------------------|--------------------------------|----------------------------|
| sharedrive_location | Path of the nfs share location | nfs.example.com:/mnt/share |

Dependencies
------------

N/A

Example Playbook
----------------
```yml
- hosts: servers
  roles:
    - role: lebergarrett.ansible_nfs_client
      vars:
        sharedrive_location: nfs.example.com:/mnt/share
```


License
-------

BSD
