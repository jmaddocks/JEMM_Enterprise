# -*- mode: ruby -*-
# vi: set ft=ruby :

masterIP = "192.168.1.122"
agent1ip = "192.168.1.123"
agent2ip = "192.168.1.124"
agent3ip = "192.168.1.125"
agent4ip = "192.168.1.126"
agent5ip = "192.168.1.127"

Vagrant.configure("2") do |config|
	config.vm.boot_timeout = 400
	
	config.vm.define "master" do |master|
		master.vm.synced_folder "shared", "/tmp/shared"
		master.vm.hostname = "JEMMEmaster.qac.local"
		master.vm.box	   = "chad-thompson/ubuntu-trusty64-gui"
		master.vm.network "public_network", ip: masterIP
		#master.vm.provision :shell, path: "bootstrap_m.sh"
		master.vm.provider :virtualbox do |masterE|
			masterE.gui    = true
			masterE.name   = "master"
			masterE.memory = 2048
			masterE.cpus   = 2
		end
	end

	config.vm.define "agent1" do |agent1|
		agent1.vm.hostname = "Jemmeagent1.qac.local"
		agent1.vm.box 	   = "chad-thompson/ubuntu-trusty64-gui"
		agent1.vm.network "public_network", ip: agent1ip
		#agent1.vm.provision :shell, path: "bootstrap_a.sh"
		agent1.vm.provider :virtualbox do |agent1e|
			agent1e.gui    = true
			agent1e.name   = "agent1e"
			agent1e.memory = 1024
			agent1e.cpus   = 2
		end
	end

	config.vm.define "agent2" do |agent2|
		agent2.vm.hostname = "Jemmeagent2.qac.local"
		agent2.vm.box = "chad-thompson/ubuntu-trusty64-gui"
		agent2.vm.network "public_netowrk", ip: agent2ip
		#agent2.vm.provision :shell, path: "bootstrap_a.sh"
		agent2.vm.provider :virtualbox do |agent2e|
			agent2e.gui    = true
			agent2e.name   = "agent2Enterprise"
			agent2e.memory = 1024
			agent2e.cpus   = 2
		end
	end

	config.vm.define "agent3" do |agent3|
		agent3.vm.hostname = "Jemmeagent3.qac.local"
		agent3.vm.box = "chad-thompson/ubuntu-trusty64-gui"
		agent3.vm.network "public_network", ip: agent3ip
		#agent3.vm.provision :shell, path: "bootstrap_a.sh"
		agent3.vm.provider :virtualbox do |agent3e|
			agent3e.gui    = true
			agent3e.name   = "agent3Enterprise"
			agent3e.memory = 1024
			agent3e.cpus   = 2
		end
	end

	config.vm.define "agent4" do |agent4|
		agent4.vm.hostname = "Jemmeagent4.qac.local"
		agent4.vm.box = "chad-thompson/ubuntu-trusty64-gui"
		agent4.vm.network "public_netowrk", ip: agent4ip
		#agent4.vm.provision :shell, path: "bootstrap_a.sh"
		agent4.vm.provider :virtualbox do |agent4e|
			agent4e.gui    = true
			agent4e.name   = "agent4Enterprise"
			agent4e.memory = 1024
			agent4e.cpus   = 2
		end
	end
	
	config.vm.define "agent5" do |agent5|
		agent5.vm.hostname = "Jemmeagent5.qac.local"
		agent5.vm.box = "chad-thompson/ubuntu-trusty64-gui"
		agent5.vm.network "public_netowrk", ip: agent5ip
		#agent5.vm.provision :shell, path: "bootstrap_a.sh"
		agent5.vm.provider :virtualbox do |agent5e|
			agent5e.gui    = true
			agent5e.name   = "agent5Enterprise"
			agent5e.memory = 1024
			agent5e.cpus   = 2
		end
	end
end

