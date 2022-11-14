OPNsense: Theme
===============

An Ansible role that allows you to configure the UI theme on an opnSense firewall.

Requirements
------------

This role requires the `lxml` python package to be installed on the host system.

Role Variables
--------------

|        Variable        |  Type  |                          Description                           |
| :--------------------: | :----: | :------------------------------------------------------------: |
|  opnsense_theme_name   | string | The name of the theme as it would have been set in the web UI. |

Dependencies
------------

N/A.

Example Playbook
----------------

```yaml
- name: Configure the web UI theme on all firewalls
  hosts: opnsense

  roles:
    - role: mirceanton.opnsense_theme
      vars:
        opnsense_theme_name: cicada
```

License
-------

MIT

Author Information
------------------

A role developed by [Mircea-Pavel ANTON](https://www.mirceanton.com).
