Apigee OPDK Region Settings
=========

This role updates the Ansible cache with attributes that are used to generate templates and make 
installation decisions. 

This role will set the region of the node that it is run on. The attributes `region` and `region_num`
are set for use in configuration files and logic in other roles. 

Requirements
------------

The data center (`dc`) must be defined as a group in the inventory file.  A `dc` must be defined as 
an inventory group such as `[dc-1]`.

Role Variables
--------------

A node that is placed in inventory group `[dc-1]` will be return a `region=dc-1` and `region_num=1`.

Dependencies
------------

N/A


Example Playbook
----------------

    - hosts: rmp
      roles:
         - { role: apigee-opdk-settings-region }

License
-------

Apache 2.0

Author Information
------------------

Carlos Frias
