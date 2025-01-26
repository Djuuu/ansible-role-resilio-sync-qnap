Ansible Role: Resilio-Sync-QNAP
===============================

Install or update Resilio Sync on QNAP NAS.

- https://www.resilio.com/sync/
- https://help.resilio.com/hc/en-us/articles/206178964-QNAP

Requirements
------------

A QNAP NAS.

Role Variables
--------------

Available role variables are listed below, along with default values (see `defaults/main.yml`):

```yaml
# Download directory for qpkg package
resilio_downoad_dir: /tmp
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: all

  gather_facts: true
  gather_subset:
    - "!all"
    - "!min"
    - architecture

  roles:
    - djuuu.resilio_sync_qnap
```

License
-------

Beerware License
