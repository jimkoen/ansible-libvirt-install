libvirt-install
=========

This role aims to get hosts into a state where they can be provisioned by the [community.libvirt](https://galaxy.ansible.com/community/docker?extIdCarryOver=true&sc_cid=701f2000001OH7YAAW) collection.

Requirements
------------

**None** - only Ansible inbuilt modules are needed.

Role Variables
--------------

```
libvirt_install_assert_hw_virtualization_support: true | false
```
This variable enables or disables assertion of the presence of certain CPU flags that are necessary for hardware accelerated virtualization.
If enabled, the assertion will fail when these flags are not present. It may or not be possible to install libvirt without hardware virtualization
support, however mileage regarding functionality, performance and reliability may vary.

Dependencies
------------

None.

Example Playbook
----------------

<!--Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      tasks:
        - include_role:
            name: libvirt-install
-->
License
-------

BSD-3-Clause

Author Information
------------------
Lucca Jiménez Könings
lucca.koenings@stud.h-da.de
Volunteer DevOps assistance role at [Hochschule Darmstadt (h_da)](https://fbi.h-da.de/), though mainly develops these roles in their free time.
