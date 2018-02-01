## Vagrantfile 

```Ruby
# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "debian7-openresty"
  config.vm.box_url = "https://github.com/jiko/OpenResty-Vagrant/releases/download/1.5.8.1/debian7-openresty.box"

  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.network "private_network", ip: "192.168.33.10"

  config.vm.synced_folder "./", "/vagrant", type: "nfs"
  config.vm.synced_folder "/opt/klear-development/", "/opt/klear-development", type: "nfs" ,
    owner: "root", group: "root"

  config.vm.provision "ansible" do |ansible|
     ansible.playbook = "Provision/playbook.yml"
     ansible.tags = ENV['ANSIBLE_TAGS']
     ansible.verbose = "vvvv"
  end

  #Especificar el número de CPUs
  config.vm.provider "virtualbox" do |v|
    v.customize ["modifyvm", :id, "--cpus", 4]
  end

end
```