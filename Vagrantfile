Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.hostname = "centos7.company.com"
  config.vm.network "private_network", ip: "192.168.33.10"

 # config.vm.provider "virtualbox"
  config.vm.provider "virtualbox" do |lvm|
    lvm.memory = '2048'
    lvm.cpus = "2"
#    lvm.storage :file, :size => '20G'
#    lvm.storage :file, :size => '40G'
  end
  config.vm.provision "shell", path: "/home/light/lab/vagrant/bootstrap.sh"
end
