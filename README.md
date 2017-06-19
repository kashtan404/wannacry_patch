wannacry_patch
=========

This role can be used for fix wannacry vulnerable.

Requirements
------------

This role requires Ansible 1.2 or higher, and platform requirements are listed in the metadata file.
Extract .cab files from .msu packages to role direcroty "files".
Cab list:
Windows6.0-KB4012598-x64.cab   - Server 2008
Windows6.1-KB4012212-x64.cab   - Server 2008 R2
Windows8-RT-KB4012214-x64.cab  - Server 2012
Windows8.1-KB4012213-x64.cab   - Server 2012 R2
Windows10.0-KB4013429-x64.cab  - Server 2016

Role Variables
--------------

do_reboot: False

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: wannacry_patch, do_reboot: True  }

License
-------

MIT

Author Information
------------------

Aleksey Demidov