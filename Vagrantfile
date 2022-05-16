
Vagrant.configure("2") do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://vagrantcloud.com/search.
  config.vm.box = "centos/7"
  config.vm.hostname = 'sonarqube'
  config.vm.network 'forwarded_port', guest: 9000, host: 9010, hostip: '127.0.0.1'
  config.vm.provision 'shell', path: 'provision.sh'
  config.vm.provider 'virtualbox' do |v|
    v.memory = 1024
  end

  
end
