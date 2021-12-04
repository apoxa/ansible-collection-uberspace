Role Name
=========

This role manages domains on an Uberspace.

Requirements
------------

None.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

| Variable  | Required | Default | Comments |
| --------  | -------- | ------- | -------- |
| `domains` | No | `[]` (Empty list) | Contains a list of Dicts with `domain` and `state` keys |
| `state` | No | `present` | This is the default state if the `domain` variable is set|
| `domain` | No | `None` | |

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: apoxa.uberspace_domain
           domain: isabell.example

License
-------

BSD
