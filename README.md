Freeswitch
=========

Ansible role for installing FreeSwitch on Debian/Ubuntu/CentOS Linux. 
For CentOS, packages from Okay repo are installed. 
For Ubuntu, packages from strukturag PPA are installed.
For Debian, packages from official Freeswitch repo are installed.

Requirements
------------

Tested on Ansible 2.8 or higher.

Role Variables
--------------

	fs_daemon: freeswitch
Defines freeswitch daemon/service name. Default: freeswitch
	fs_enabled: true
Defines whether to enable freeswitch service. Default: true
	fs_started: false
Defines whether to start freeswitch service. Default: false
	fs_install_full: false
Defines whether to install all the available freeswitch packages. Default: false


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: kbcz1989.ansible-role-freeswitch }

License
-------

MIT

Author Information
------------------

KBCZ1989
