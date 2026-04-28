# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|

  config.vm.define "rocky" do |rocky_config|
    rocky_config.vm.box = "bento/rockylinux-10"
    rocky_config.vm.box_version = "202512.01.0"
    rocky_config.vm.hostname = "rockylinux10"
    rocky_config.vm.provider "virtualbox" do |vb|
      vb.name = "rockylinux10"
      vb.cpus = 4
      vb.memory = 8192
    end

  config.vm.define "alma" do |alma_config|
    alma_config.vm.box = "almalinux/10"
    alma_config.vm.box_version = "10.1.20260318"
    alma_config.vm.hostname = "alma"
    alma_config.vm.provider :libvirt do |libvirt|
      libvirt.cpus = 4
      libvirt.memory = 8192
      libvirt.machine_type = "q35"
      libvirt.driver = "kvm"
    end
end

