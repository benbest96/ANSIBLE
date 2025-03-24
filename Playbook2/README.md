First Ansible Playbook Demo VM
----------------------------------------

This project spins up a VM and demonstrates a very simple Ansible playbook.

Quick Start Guide
1 - Install dependencies (VirtualBox, Vagrant, Ansible)
Download and install VirtualBox.
Download and install Vagrant.
[Mac/Linux only] Install Ansible.
Note for Windows users: This guide assumes you're on a Mac or Linux host. Windows hosts are unsupported at this time.

2 - Build the Virtual Machine
Download this project and put it wherever you want.
Open Terminal, cd to this directory.
Type in vagrant up, and let Vagrant do its magic.
Note: If there are any errors during the course of running vagrant up, and it drops you back to your command prompt, just run vagrant provision to continue building the VM from where you left off. If there are still errors after doing this a few times, post an issue to this project's issue queue on GitHub with the error.

Notes
To shut down the virtual machine, enter vagrant halt in the Terminal in the same folder that has the Vagrantfile. To destroy it completely (if you want to save a little disk space, or want to rebuild it from scratch with vagrant up again), type in vagrant destroy.
About the Author
This project was created by Jeff Geerling as an example for Ansible for DevOps.