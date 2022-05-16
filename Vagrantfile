# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
  config.vm.box = "generic/ubuntu2004"
  config.vm.network "private_network", ip: "192.168.56.56"
  config.ssh.insert_key = false 
  config.vm.provision :shell, :inline => "sudo rm /etc/localtime && sudo ln -s /usr/share/zoneinfo/Europe/Moscow /etc/localtime", run: "always"
  config.vm.network "forwarded_port", guest: 3000, host: 3000
  config.vm.synced_folder "./homework/", "/home/vagrant/homework/", type: "rsync"
  config.vm.provision "ansible" do |ansible|
  #ansible.verbose = "v"
  ansible.playbook = "hw.yml"
  end
end
