# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "desarrollo-seguro/xfce4"

  # config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"

  # Create a private network, which allows host-only access to the machine
  # using a specific IP.
  # config.vm.network "private_network", ip: "192.168.33.10"

  # Create a public network, which generally matched to bridged network.
  # Bridged networks make the machine appear as another physical device on
  # your network.
  # config.vm.network "public_network"

  config.vm.provider "virtualbox" do |vb|
     vb.gui = true
     vb.memory = "3072"
     vb.cpus = 2
  end

  config.vm.provision "shell", inline: "sudo apt-get update"
  config.vm.provision "shell", inline: "sudo apt-get upgrade -y"
end
