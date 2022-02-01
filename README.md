OpenWRT_dropbear_authorizedkeys
=========

Put a public SSH key into /etc/dropbear/authorized_keys on a OpenWrt machine

Requirements
------------

None.

Role Variables
--------------

- `ssh_pub_key_location`: Path to the public key file to be used, defaults to `$HOME/.ssh/.ssh/id_rsa.pub` on the Ansible controller machine

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
