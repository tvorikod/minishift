# -*- mode: ruby -*-
# vi: set ft=ruby :

ENV['VAGRANT_DEFAULT_PROVIDER'] = 'libvirt'
Vagrant.configure(2) do |cnfg|
  cnfg.vm.define 'minishift-vm' do |mvm|
    mvm.vm.box = 'centos/7'
    mvm.vm.box_url = mvm.vm.box
    mvm.vm.provider 'libvirt' do |prv|
      prv.nested = true
      prv.memory = 4096
      prv.cpus = 2
  end
end
