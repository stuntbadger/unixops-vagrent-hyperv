Vagrant.configure("2") do |config|
  config.vm.box = "generic/rocky9"
   config.vm.provider "hyperv" do |vb, override|
     vb.cpus = 2 
     vb.maxmemory = 4096
     vb.memory = 4096
     vb.vmname = "unixops"
   end
   config.vm.provision "shell", path: "scripts/install.sh"
   config.vm.hostname = "unixops-local"
end
