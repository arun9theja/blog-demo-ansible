# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure("2") do |config|



  config.vm.box = "p0bailey/xenial64"

  config.vm.network "private_network", type: "dhcp"


  config.vm.provision "shell", inline: <<-SHELL
    chmod +x /vagrant/ansible_provision.yml
    /vagrant/ansible_provision.yml
  SHELL

end
