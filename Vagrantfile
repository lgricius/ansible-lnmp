Vagrant.configure(2) do |config|
    config.vm.box = "precise32"
        config.vm.box_url = "http://files.vagrantup.com/precise32.box"
    config.vm.network "private_network", ip: "123.123.123.123"
    config.vm.provision "ansible" do |ansible|
        ansible.verbose = 'vv'
        ansible.limit = 'all'
        ansible.playbook = "provisioning/playbook.yml"
    end
end
