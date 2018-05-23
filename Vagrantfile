# -*- mode: ruby -*-
# vi: set ft=ruby :

# README
#
# Getting Started:
# 1. vagrant plugin install vagrant-hostmanager
# 2. vagrant up
# 3. vagrant ssh
#
# This should put you at the control host
#  with access, by name, to other vms
Vagrant.configure(2) do |config|
  config.hostmanager.enabled = true

  config.vm.box = "ubuntu/xenial64"
  config.vm.box_url = "/home/ichank/Documents/ubuntu1604.box"

  config.vm.define "docker", primary: true do |h|
    h.vm.network "private_network", ip: "192.168.136.10"
  end
end