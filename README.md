SourceGuardian
==============

A Role to install Source Guardian (licensed) encoder or loader on rhel/CentOS/Fedora servers.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```yaml
    sg_version: 11      # Defines source-guardian version
    sg_arch: x86_64     # Defines source-guardian architecture
    sg_install_encoder: # Install source-guardian lisenced encoder
    sg_install_loader:  # Install source-guardian's loader only (lisenced by SourceGuardian)
```

Dependencies
------------

None.

Example Playbook
----------------

Here's an example playbook with few variables:

```yaml
- hosts: apps-server
  vars:
    sg_version: 11
    sg_install_encoder: True
  roles:
     - name: laxathom.sourceguardian
```

License
-------

MIT
