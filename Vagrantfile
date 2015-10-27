# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = 'ubuntu/trusty64'
  config.cache.scope = :box if Vagrant.has_plugin?("vagrant-cachier")
  config.vm.provision :ansible do |ansible|
    ansible.playbook = 'playbook.yml'
  end
end
