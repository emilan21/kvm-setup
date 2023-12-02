kvm-setup
=========

Role will setup a Ubuntu 23.04 server to be a kvm host

Requirements
------------

None

Role Variables
--------------

Currently the following variables are required and expected to be pass via the playbook that includes the role

user: User account.
public_ssh_key_for_domains: Public ssh key that will be put into the domain images. Might move this to the provisioning role
interface: Real interface
bridge_interface: Bridge interface
addresses: ipv4 address in this format x.x.x.x/x so 192.168.1.5/24
macaddress: Mac address of interface
default_route: Default gateway
nameservers: dns servers

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

MIT

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
