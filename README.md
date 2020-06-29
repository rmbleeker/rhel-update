rhel-update
===========

Update Red Hat systems

Requirements
------------

None

Role Variables
--------------

```
yum_exclude_packages: list of packages that should not be updated
security_updates_only: only apply security updates, no system updates
```

Example:
```
    yum_exclude_packages:
      - kernel*
      - foo*
```

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - rhel-update

License
-------

BSD

Author Information
------------------

Ruud Bleeker
