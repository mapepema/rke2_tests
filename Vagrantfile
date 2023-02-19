# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.ssh.forward_agent = true

  config.vm.define "master" do |master|
    master.vm.box = "generic/opensuse42"
    master.vm.network "public_network"
    master.vm.provider "virtualbox" do |vb_master|
      vb_master.gui = false
      vb_master.memory = "4096"
      vb_master.cpus = 4
    end
  end

  config.vm.define "worker" do |master|
    master.vm.box = "generic/opensuse42"
    master.vm.network "public_network"
    master.vm.provider "virtualbox" do |vb_worker|
      vb_worker.gui = false
      vb_worker.memory = "4096"
      vb_worker.cpus = 4
    end
  end

end
