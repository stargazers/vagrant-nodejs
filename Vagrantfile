# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

    config.vm.box = "ubuntu/xenial64"
    config.vm.box_check_update = false

    config.vm.network "forwarded_port", guest: 80, host: 8080
    config.vm.network "private_network", bridge: "en1: Wi-Fi (AirPort)", ip: "10.1.1.100"

    config.vm.provider "virtualbox" do |vb|
        vb.memory = "2048"
    end

    config.vm.provision :ansible do |ansible|
        ansible.playbook = "playbooks/install-nodejs.yml"
    end
end
