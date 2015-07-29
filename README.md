Role Name
=========

Installs dnsmasq http://www.thekelleys.org.uk/dnsmasq/doc.html

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

````
config_dnsmasq: false  #defines if DNSMASQ should be configured
dnsmasq_misc_backup_dir: []
dnsmasq_misc_home: []
enable_dnsmasq_dhcp: false  #defines if DHCP services are provided by DNSMASQ
enable_dnsmasq_dhcp_tftp: false  #defines if DHCP and TFTP services are provided by DNSMASQ
enable_tftp: false  #defines if TFTP services are provided by DNSMASQ
pri_domain_name: example.org
sync_dnsmasq: false  #defines if DNSMASQ is synced between nodes when using GlusterFS
````

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: mrlesmithjr.dnsmasq }

License
-------

BSD

Author Information
------------------

Larry Smith Jr.
- @mrlesmithjr
- http://everythingshouldbevirtual.com
- mrlesmithjr [at] gmail.com
