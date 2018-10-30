
Vagrant.configure("2") do |config|
  
  config.vm.box = "sscf-box"
  
  #config.vm.network "forwarded_port", guest: 22, host: 2222, id:'ssh', disabled:'true'
  #config.vm.network "forwarded_port", guest: 22, host: 22156

  config.vm.network "forwarded_port", guest: 3306, host: 3306
  
  # 指定虚拟机的IP
  #config.vm.network "public_network", ip: "192.168.11.156"
  
  # 貌似这个好用，上面那个公共网络有时候不行，设置了这个，用于访问网站；管理服务器还是使用127.0.0.1:2222（默认情况下）
  # 可以不同网段，比如主机IP是192.168.11.156，设置下面这个也是可以访问的
  config.vm.network "private_network", ip: "192.168.0.101"

  # 将windows上的文件夹映射到虚拟机上
  config.vm.synced_folder "E:\\test", "/home/test"
  
  # 指定用户名和密码
  config.ssh.username = "vagrant"
  config.ssh.password = "vagrant"
end
