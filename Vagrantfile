# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ESCRIBA_EL_BOX"
  config.vm.define "web01" do |web|
  	web.vm.provider :virtualbox do |vb|
		vb.customize [ 'modifyvm', :id, '--memory', '386' ]
		vb.customize [ 'modifyvm', :id, '--cpus', '1' ]
		vb.customize [ 'modifyvm', :id, '--name', 'web01' ]
  	end
  end
  config.vm.define "web02" do |web|
  	web.vm.provider :virtualbox do |vb|
		vb.customize [ 'modifyvm', :id, '--memory', '386' ]
		vb.customize [ 'modifyvm', :id, '--cpus', '1' ]
		vb.customize [ 'modifyvm', :id, '--name', 'web02' ]
  	end
  end
  config.vm.define "haproxy" do |hap|
  	hap.vm.provider :virtualbox do |vb|
		vb.customize [ 'modifyvm', :id, '--memory', '386' ]
		vb.customize [ 'modifyvm', :id, '--cpus', '1' ]
		vb.customize [ 'modifyvm', :id, '--name', 'hap' ]
  	end
  end
end
