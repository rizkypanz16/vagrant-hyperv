Vagrant.configure("2") do |config|

  config.vm.box = "vagrant-ubuntu22.04"

  config.vm.provider "hyperv" do |hv|
    hv.vmname = "vagrant-dockernode"
    hv.cpus = 2
    hv.memory = 4000
  end

  config.vm.hostname = "vagrant-dockernode"
  
  # Specify the external virtual switch name
  config.vm.network :public_network, bridge: 'External Switch'


  # Disable SMB shared folders
  config.vm.synced_folder '.', '/vagrant', disabled: true

end

