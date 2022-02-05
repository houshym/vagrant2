Vagrant.configure("2") do |config|
   (1..3).each do |i|

      config.vm.define "node#{i}" do |node|

      node.vm.box = "ubuntu/xenial64"

      node.vm.hostname = "node#{i}"

      node.vm.network "private_network", ip: "192.168.100.#{110+i}"


      node.vm.provider "virtualbox" do |v|


          v.name = "node#{i}"


          v.memory = 4096


          v.cpus = 4
      end
  end
end
end
