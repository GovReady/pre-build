Pre-Build
=============================

Pre-Build is an empty, GitMachine with GovReady components to pre-build an intented GovReady GitMachine.


## How to Use

Before building any GovReady GitMachine, it is a good idea to launch a barebones VM and follow a set of manual instructions to build and configure the system. This the barebones VM to use.


## Advantages

Using a virtual machines to test software has many advantages

* It's more secure: you are not installing anything on your computer.
* You don't have to change your computer's configuration to test install new software.
* Virtual machines can be thrown away and when you mess up.
* You can use DevOps tools to automate configuring software on a VM.
* You can share your automation and even the entire virtual machine.

## Background

## What's on this Pre-Build, barebones machine?

* CentOS 6.4
* Apache
* PHP
* Simple Ansible playbook to install
* Apache
* PHP
* GovReady toolkit (alpha)

## Links

### Ansible
* [Jeff Geerling Slides](http://www.slideshare.net/geerlingguy/local-development-on-virtual-machines-vagrant-virtualbox-and-ansible)
* [Ansible's Example on GitHub](https://github.com/ansible/ansible-examples/tree/master/lamp_simple)
* [Julian Ponge post with examples](http://julien.ponge.org/blog/scalable-and-understandable-provisioning-with-ansible-and-vagrant/)
* [Ansible docs on using Vagrant](http://docs.ansible.com/guide_vagrant.html)
* [Vagrant docs on using Ansible](http://docs.vagrantup.com/v2/provisioning/ansible.html)
* [Getting Cirrius example of Ansible and Firewall rules](http://www.gettingcirrius.com/2013/11/configure-iptables-with-ansible.html)
* [CentOS wiki EC2 and Ansible](http://wiki.centos.org/Cloud/Manage/Ansible)

More on Ansible
* Ansible executes in order.
* Ansible playbook needs to address `hosts`, `vars`, `handlers`, and `tasks`. 
* Variable substitution in Ansible `{{ var_name }}` 
* Ansible loop you indicate the command and then add `with_items` YAML list. 
* Ansible copy file by defaults copies `src` from Ansible computer to `dest` on guest (target) server. You can set mode and ownership
* Copying files really is an easy way manage firewalls and vhost configurations.


