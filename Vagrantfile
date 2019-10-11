# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
config.ssh.insert_key = false
  config.vm.define "acs" do |acs|
    acs.vm.box = "centos/7"
	acs.vm.hostname = "acs"
	acs.vm.network "private_network", ip: "192.168.33.10"
  end
  config.vm.define "app" do |web|
    web.vm.box = "centos/7"
	web.vm.hostname = "app"
	web.vm.network "private_network", ip: "192.168.33.20"
  end
  config.vm.define "db" do |db|
    db.vm.box = "centos/7"
	db.vm.hostname = "db"
	db.vm.network "private_network", ip: "192.168.33.30"
  end
    config.vm.define "tac" do |db|
    db.vm.box = "centos/7"
	db.vm.hostname = "tac"
	db.vm.network "private_network", ip: "192.168.33.40"
  end
end
	