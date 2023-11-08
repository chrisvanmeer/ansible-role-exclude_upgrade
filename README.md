ansible-role-exclude_upgrade
=========

Exclude packages from upgrades

Requirements
------------

The defined packages you want to exclude must be installed on the target host.

Role Variables
--------------

```
exclude_upgrade_packages: []
```

See example for usage.


Dependencies
------------

No dependencies.

Example Playbook
----------------

```
- hosts: server
  become: true

  roles:
    - role: exclude_upgrades
      exclude_upgrade_packages:
        - consul-enterprise
        - vault-enterprise
        - nomad-enterprise
```

License
-------

EUPL-1.2

Author Information
------------------

- Chris van Meer <c.v.meer@atcomputing.nl>
