Role Name
=========

- creates bridges for single-nic-vlan configuration
- creates n vms

Role Variables
--------------


bridges:
  - br-vlans:
    name: br-vlans
    member_nic: enp1s0f1
    disable_ageing: True

vm_name_prefix: overcloud
vm_disk_size: 30G
guest_vms_count: 10
vms_image_location: /vms

overcloud_node:
  memory: 6
  vcpu: 2

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables
passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: ansible-kvm-vm

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a
website (HTML is not allowed).
