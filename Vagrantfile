Vagrant.configure('2') do |config|
  config.vm.box = "centos/7"
  config.vm.provider "virtualbox" do |v|
    v.name = "jenkins-lab"
    v.memory = 2048
    v.cpus = 2
  end
  config.vm.synced_folder ".", "/vagrant", automount: true
  # config.vm.synced_folder "roles/", "/etc/ansible/roles", automount: true
  # config.vm.network "private_network", type: "dhcp", virtualbox__intnet: "vboxnet0"
  config.vm.network "private_network", ip: "192.168.56.200"#, virtualbox__intnet: "vboxnet0"
  config.vm.provision "ansible_local" do |ansible|
    # ansible.inventory_path = "/vagrant/hosts"
    ansible.galaxy_roles_path = "/vagrant/roles"
    ansible.playbook = "playbook.yml"
  end
end