# OUTDATED Repo


## Ansible VMcreator
Ansible Playbook to quickly roll out a set of virtual machines on libvirt

what does it do:
* thin clone VM-boot Disk from an RHEL7 Template using qemu-img with backing store
* creates a second disk for each VM if requested
* uses libguestfs tools to inject static network config into VMs
* creates the VM definition from J2-templated XML-file

requires:
* qemu-kvm, libvirt
* libuestfstools

Work in progress:
* build as role
* add more variables to make the vmcreator Playbook more flexible
* add more Playbooks to configure the VMs after being rolled out
