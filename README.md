![Ansible Lint](https://github.com/johanneskastl/ansible-role-OpenWRT_dropbear_authorizedkeys/workflows/Ansible%20Lint/badge.svg)

OpenWRT_dropbear_authorizedkeys
=========

Put a public SSH key into `/etc/dropbear/authorized_keys` on a OpenWrt machine.

Requirements
------------

None.

Role Variables
--------------

You have two options:

In case you only need one key added to the `authorized_keys` file, use `ssh_pub_key_location`.

- `ssh_pub_key_location`: Path to the public key file to be used, defaults to `~/.ssh/id_rsa.pub` on the Ansible controller machine

In case there are multiple keys you want to add, use `multiple_ssh_pub_key_locations`:

- `multiple_ssh_pub_key_locations`: list of strings, where each contains the path to a SSH publich key file.

Please note that this variable does not have a default value.

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
        - { role: 'johanneskastl.OpenWRT_dropbear_authorizedkeys' }

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via kastl@b1-systems.de.
