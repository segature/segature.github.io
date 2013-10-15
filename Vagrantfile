Vagrant::Config.run do |config|
	config.vm.box = "precise64"
	config.vm.box_url = "http://files.vagrantup.com/precise64.box"
	config.vm.host_name = "segature-octopress"
	
	config.vm.provision :shell, :path => "bootstrap.sh"
	config.vm.share_folder("vagrant-root", "/vagrant", ".", :extra => 'dmode=777,fmode=777')
end