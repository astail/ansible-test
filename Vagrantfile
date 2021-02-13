AGRANTFILE_API_VERSION = "2"

Vagrant.configure("2") do |config|
  config.vm.box = "bento/amazonlinux-2"
  config.ssh.insert_key = false
  config.vm.provider "virtualbox" do |vm|
#    vm.cpus = 2
    vm.memory = 1024
  end

  config.vm.define "node01" do |node|
    node.vm.hostname = "node01"
    node.vm.network "private_network", ip: "192.168.34.21"
  end

  config.vm.define "node02" do |node|
    node.vm.hostname = "node02"
    node.vm.network "private_network", ip: "192.168.34.22"
  end
end
