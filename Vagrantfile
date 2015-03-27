box      = 'phusion/ubuntu-14.04-amd64'
version  = 2

Vagrant.configure(version) do |config|
  config.vm.box = box
	
	config.vm.provision :shell, :inline => "apt-get -qy update"
	config.vm.provision :shell, :inline => "apt-get -qy install software-properties-common python-software-properties"
	config.vm.provision :shell, :inline => "add-apt-repository ppa:openjdk-r/ppa"
	config.vm.provision :shell, :inline => "apt-get -qy update"	
  config.vm.provision :shell, :inline => "apt-get -qy install openjdk-8-jdk"
	
end
