Vagrant.configure("2") do |config|

  config.vm.define "acs" do |acs|
    acs.vm.box = "ubuntu/trusty64"
    acs.vm.hostname = "ansible"
    acs.vm.network "private_network", ip: "192.168.1.50"
  
    acs.vm.provision "ansible_local" do |ansible|
      ansible.playbook = "test.yml"
    end
  end
end
