
Vagrant.configure("2") do |config|
  
  config.vm.box = "sscf-box"
  config.vm.network "forwarded_port", guest: 22, host: 2222, id:'ssh', disabled:'true'
  config.vm.network "forwarded_port", guest: 22, host: 22156

  # 指定虚拟机的IP
  config.vm.network "public_network", ip: "192.168.11.156"

  # 将windows上的文件夹映射到虚拟机上
  config.vm.synced_folder "E:\\test", "/home/test"
  
  # 指定用户名和密码
  config.ssh.username = "vagrant"
  config.ssh.password = "vagrant"
end
