
Vagrant.require_version ">=1.9.0"

Vagrant.configure("2") do |config|

  config.vm.define vm_name="ubutrustypostgres" do |server|

    server.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 1
      vb.name = vm_name
      vb.memory = 1024
    end

    server.vm.hostname = vm_name
    server.vm.box = "ubuntu/trusty64"
    server.vm.network "forwarded_port", guest: 5432, host: 5432

    server.vm.provision :shell, path: "provision_postgresql94.sh"
    #server.vm.provision :shell, path: "provision_postgresql95.sh"

  end

end
