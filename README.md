Just a basic docker-nginx role that was extracted from a monorepo.

Bare host
---------

Deploy a docker-based self-configuring nginx with letsencrypt support:

    bigsudo yourlabs.nginx --become -v @somehost

Vagrant/VirtualBox
------------------

You can work in a VM if you have vagrant:

    cd yourlabs.nginx
    vagrant destroy -f && vagrant up
    vagrant ssh-config > ssh
    bigsudo . --ssh-common-args="-F ssh" @default --become -v
