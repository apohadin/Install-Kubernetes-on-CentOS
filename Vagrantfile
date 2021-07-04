# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.define "master" do |master|
    master.vm.box_download_insecure = true
    master.vm.box = "bento/centos-7"
    master.vm.network "private_network", ip: "192.168.56.100"
    master.vm.hostname = "master"
    master.vm.provider "virtualbox" do |v|
      v.name = "master"
      v.memory = 2048
      v.cpus = 2
    end
  end

  config.vm.define "worker1" do |worker1|
    worker1.vm.box_download_insecure = true
    worker1.vm.box = "bento/centos-7"
    worker1.vm.network "private_network", ip: "192.168.56.200"
    worker1.vm.hostname = "worker1"
    worker1.vm.provider "virtualbox" do |v|
      v.name = "worker1"
      v.memory = 1024
      v.cpus = 1
    end
  end

  config.vm.define "worker2" do |worker2|
    worker2.vm.box_download_insecure = true
    worker2.vm.box = "bento/centos-7"
    worker2.vm.network "private_network", ip: "192.168.56.201"
    worker2.vm.hostname = "worker2"
    worker2.vm.provider "virtualbox" do |v|
      v.name = "worker2"
      v.memory = 1024
      v.cpus = 1
    end
  end


end

