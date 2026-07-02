# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|

  config.vm.define "alma" do |alma_config|
    alma_config.vm.box = "almalinux/9"
    alma_config.vm.box_version = "9.8.20260526"
    alma_config.vm.hostname = "alma"
    alma_config.vm.provider :libvirt do |libvirt|
      libvirt.cpus = 4
      libvirt.memory = 4096
      libvirt.machine_type = "q35"
      libvirt.driver = "kvm"
    end
  end

end
