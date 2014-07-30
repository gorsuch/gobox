# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = '2'

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.hostname = 'gobox'
  config.vm.box = 'chef/debian-7.4'

  config.vm.provision 'ansible' do |ansible|
    ansible.playbook = 'vagrant.yml'
  end
end
