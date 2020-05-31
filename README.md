ansible-role-fish
=================

A simple role to install and configure the fish shell on remote systems

Requirements
------------

This role expects to work on a Mac or Linux system. It only works for the user defined in `ansible_user`.

Role Variables
--------------

* `set_default_shell`
  * Type: Boolean
  * Usage: If `true`, sets fish as the default shell for `ansible_user`.
  * Default: `false`

Dependencies
------------

This role has no dependencies of note.

Example Playbook
----------------

```yaml
- hosts: local
  roles:
    - fish
  vars:
    fish:
      set_default_shell: true
```

License
-------

MIT

Author Information
------------------

Patrick Wagstrom &lt;patrick@wagstrom.net&gt;