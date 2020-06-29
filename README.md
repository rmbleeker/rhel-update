rhel-update
===========

Update Red Hat systems

Requirements
------------

None

Role Variables
--------------

```(yaml)
yum_exclude_packages:   # list of packages that should not be updated
reboot_when:            # the number of **minutes** to wait for a system restart
security_updates_only:  # only apply security updates, no system updates
```

Example:
```(yaml)
    yum_exclude_packages:
      - kernel*
      - foo*
```

Dependencies
------------

None

Example Playbook
----------------

```(yaml)
    - hosts: servers
      roles:
         - rhel-update
```

License
-------

BSD

Author Information
------------------

Ruud Bleeker
