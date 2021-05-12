# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "generic/rhel8"
  config.vm.hostname = "lab.vm1"
  config.vm.network :private_network, ip: "192.168.55.55"
  config.ssh.insert_key = false
  config.vm.synced_folder ".", "/vagrant", disabled: true

  config.vm.provider :virtualbox do |v|
    v.memory = 512 
    v.cpus = 1

    (0..2).each do |i|
      v.vm.disk :disk, size: "5GB", name: "disk-#{i}"
  end

end