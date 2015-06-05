correcthorse.vagrantbox
=========

This is a role to help prepare a virtual machine for conversion into a vagrant box. It takes care of a few common tasks like creating the vagrant user, setting up the expected insecure passwords/keys and installing some basic build tools that are needed to install virtual machine additions.

Role Variables
--------------
| Variable				| Default			|				|
| :---					| :---				| :---				|
| vagrantbox_vagrant_user		| vagrant			|				|
| vagrantbox_vagrant_home		| /home/vagrant			|				|
| vagrantbox_set_password		| true				|				|
| vagrantbox_crypted_password		| $6$rounds=40000$fCtQS1S1Uj8IylvT$YVL9k3gIlh.mk6USDf6ZXQRVk8DilUEUAdSRqwdgFAaup00QhQgTf1ABuFAjtc9HS1sxjHEcNbefNqjEDAeAs1   | |
| vagrantbox_public_key			| vagrant.pub			|				|
| vagrantbox_hypervisor			| virtualbox			|				|
| vagrantbox_install_tools		| true				|				|
| vagrantbox_disable_selinux		| true				|				|

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: correcthorse.vagrantbox }

License
-------

MIT

Author Information
------------------

* [Joshua Rusch](https://correct.horse/)
