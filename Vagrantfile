# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
	config.vm.define "acs" do |acs|
	  acs.vm.box = "ubuntu/trusty64"
	  acs.vm.hostname = "acs"
	  acs.vm.network "private_network", ip: "192.168.33.10"
	end
	
	# config.vm.define "web" do |web|
	  # web.vm.box = "nrel/CentOS-6.5-x86_64"
	  # web.vm.hostname = "web"
	  # web.vm.network "private_network", ip: "192.168.33.20"
	  # web.vm.network "forwarded_port", guest: 80, host: 8090
	# end
	
	# config.vm.define "couchdb" do |couchdb|
	  # couchdb.vm.box = "ubuntu/trusty64"
	  # couchdb.vm.hostname = "couchdb"
	  # couchdb.vm.network "private_network", ip: "192.168.33.30"
	# end

	# config.vm.define "mariadb" do |mariadb|
	  # mariadb.vm.box = "ubuntu/trusty64"
	  # mariadb.vm.hostname = "mariadb"
	  # mariadb.vm.network "private_network", ip: "192.168.33.40"
	# end	
	
	config.vm.define "docker" do |docker|
	  docker.vm.box = "ubuntu/trusty64"
	  docker.vm.hostname = "docker"
	  docker.vm.network "private_network", ip: "192.168.33.50"
	end	
	
	# config.vm.define "npm" do |npm|
	  # npm.vm.box = "ubuntu/trusty64"
	  # npm.vm.hostname = "npm"
	  # npm.vm.network "private_network", ip: "192.168.33.60"
	  # npm.vm.network "forwarded_port", guest: 8800, host: 8800
      # npm.vm.network "forwarded_port", guest: 8080, host: 8088
      # npm.vm.network "forwarded_port", guest: 8081, host: 8081
	# end	
	
	# config.vm.define "sinopia" do |sinopia|
	  # sinopia.vm.box = "ubuntu/trusty64"
	  # sinopia.vm.hostname = "sinopia"
	  # sinopia.vm.network "private_network", ip: "192.168.33.90"
	  # sinopia.vm.network "forwarded_port", guest: 4873, host: 4873
	# end	
	
	config.vm.define "jira" do |jira|
	  jira.vm.box = "ubuntu/trusty64"
	  jira.vm.hostname = "jira"
	  jira.vm.network "private_network", ip: "192.168.33.100"
	end	
	
end