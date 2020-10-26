## Ansible VMcreator
### v2

Ansible Playbook to quickly roll out a set of virtual machines on libvirt

what does it do:
* thin clone VM-boot Disk from a given Template using qemu-img with backing store
* creates a second disk for each VM if requested (and a third if necessary)
* predefines the MAC-Adress of the VM so your DNS-Server can assign fitting IP-Adresses
* creates the VM definition from J2-templated XML-file

requires:
* qemu-kvm,
* libvirt
* (optional) DNS-Server with static "dhcp-host=<MAC>:<IP>" declarations

