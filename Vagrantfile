# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure(2) do |config|
  config.vm.box = "terrywang/archlinux"
  config.vm.provider "virtualbox" do |vb|
    vb.cpus = 4
    vb.memory = "4096"
  end

  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
