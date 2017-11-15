# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "private_network", ip: "192.168.33.30"
  config.vm.provider "virtualbox" do |vb| 
     vb.memory = "2048" 
  end 
  config.vm.provision "ansible_local" do |ansible| 
     ansible.playbook = "provisioning/playbook.yml" 
  end
end
