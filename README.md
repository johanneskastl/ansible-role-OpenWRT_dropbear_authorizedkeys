OpenWRT_dropbear_authorizedkeys
=========

Put a public SSH key into /etc/dropbear/authorized_keys on a OpenWrt machine

Requirements
------------

None.

Role Variables
--------------

None.

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
