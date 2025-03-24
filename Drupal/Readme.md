Simple Drupal Development VM
For a fully-featured Drupal VM environment, check out Drupal VM.

This project simplifies the management of local test and development environments for Drupal. It automatically installs the following on an Ubuntu virtual machine:

+ Apache

+ PHP

+ MySQL

+ Drush

+ Drupal

Building or rebuilding the VM from scratch takes approximately 5–10 minutes on a decent broadband connection.

Quick Start Guide
1 - Install Dependencies (VirtualBox, Vagrant, Ansible)
Download and install VirtualBox.

Download and install Vagrant.

[Mac/Linux only] Install Ansible.

Note for Windows users: This guide is designed for macOS and Linux. Windows support may be added later. The key difference is that Ansible must be set up from within the VM after it’s created. See JJG-Ansible-Windows for more details.

2 - Build the Virtual Machine
Download this project and place it wherever you prefer.

Open a terminal and navigate to the directory containing the Vagrantfile and this README file.

Run vagrant up and let Vagrant handle the setup.

Note: If an error occurs during vagrant up and the process stops, run vagrant provision to continue from where it left off. If errors persist after multiple attempts, report the issue on this project's GitHub page with the error details.

3 - Configure Your Host Machine to Access the VM
Modify your hosts file by adding the following line:

Open a web browser and visit http://drupal.test/.

Additional Notes
To shut down the VM, use vagrant halt in the terminal from the same directory as the Vagrantfile. To completely remove it and free up disk space, use vagrant destroy.

You can change the installed Drupal version by editing the variables in vars.yml.