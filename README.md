BigSudo/Ansible role to deploy nginx-proxy container

Vagrant/VirtualBox
------------------

You can work in a VM if you have vagrant::

   vagrant destroy -f && vagrant up
   vagrant ssh-config > ssh
   bigsudo . --ssh-common-args="-F ssh" @default
