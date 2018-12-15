# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure(2) do |config|
  config.vm.define  "awscli" do |host|
    host.vm.box = "centos/7"
    host.vm.hostname = "awscli"
    host.vm.network "private_network", ip: "192.168.50.98"
    host.vm.provision "shell", path: "strap_aws", privileged: false
  end
end
