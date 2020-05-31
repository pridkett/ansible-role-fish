ansible-role-fish
=================

A simple role to install and configure the fish shell on remote systems

Requirements
------------

This role expects to work on a Mac or Linux system. It only works for the user defined in `ansible_user`.

Role Variables
--------------

`fish,set_default_shell`: Whether or not `fish` should be set to the default shell after installation. This is only for the `ansible_user` user.

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