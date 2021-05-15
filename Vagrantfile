# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.define "srv1" do |srv1|
    srv1.vm.box = "generic/rhel8"
    srv1.vm.hostname = "vm1"
    srv1.vm.network :private_network, ip: "192.168.55.55"
    srv1.ssh.insert_key = false
    srv1.vm.synced_folder ".", "/vagrant", disabled: true
    srv3.vm.disk :disk, name: "STOR", size: "3GB"
    srv1.vm.provider :virtualbox do |res|
      res.memory = 512 
      res.cpus = 1
    end
  end

  config.vm.define "db" do |srv2|
    srv2.vm.box = "generic/rhel8"
    srv2.vm.hostname = "vm2"
    srv2.vm.network :private_network, ip: "192.168.55.56"
    srv2.ssh.insert_key = false
    srv2.vm.synced_folder ".", "/vagrant", disabled: true
    srv2.vm.disk :disk, name: "STOR", size: "3GB"
    srv2.vm.provider :virtualbox do |res|
      res.memory = 512 
      res.cpus = 1
    end
  end

  config.vm.define "db" do |srv3|
    srv3.vm.box = "generic/rhel8"
    srv3.vm.hostname = "vm2"
    srv3.vm.network :private_network, ip: "192.168.55.57"
    srv3.ssh.insert_key = false
    srv3.vm.synced_folder ".", "/vagrant", disabled: true
    srv3.vm.disk :disk, name: "STOR", size: "3GB"
    srv3.vm.provider :virtualbox do |res|
      res.memory = 512 
      res.cpus = 1
    end
  end

end