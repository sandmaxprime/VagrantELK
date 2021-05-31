# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "sandmaxprime/bionic-elk"
  config.vm.hostname = "elk7x"
  config.vm.network :forwarded_port, guest: 5601, host: 5601, id: "kibana", auto_correct: true
  config.vm.network :forwarded_port, guest: 9200, host: 9200, id: "elasticsearch", auto_correct: true
  config.vm.provision "shell", inline: <<-SHELL
    apt-get update
    apt-get upgrade -y
  SHELL
  
  config.vm.provider "virtualbox" do |vb|
     vb.gui = true
     vb.name = "ELK7x"
     vb.customize ["modifyvm", :id, "--memory", 4096]
     vb.customize ["modifyvm", :id, "--cpus", 2]
  end

end
