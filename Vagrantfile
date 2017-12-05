# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.define "ubuntu" do |ubuntu|
    ubuntu.vm.box = "ubuntu/xenial64"
    ubuntu.vm.provider "virtualbox" do |virtualbox|
      virtualbox.memory = 1024
    end
  end

  config.vm.define "debian" do |debian|
    debian.vm.box = "debian/stretch64"
    debian.vm.provider "virtualbox" do |virtualbox|
      virtualbox.memory   = 1024
    end
  end
end
