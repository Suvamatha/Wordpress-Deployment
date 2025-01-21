Vagrant.configure("2") do |config|
  # WordPress VM
  config.vm.define "wordpress" do |wordpress|
    wordpress.vm.box = "ubuntu/jammy64"
    wordpress.vm.network "private_network", ip: "192.168.56.101"
    wordpress.vm.provision "shell", inline: <<-SHELL
      sudo apt update
      sudo apt install -y apache2 php php-mysql libapache2-mod-php unzip
      sudo systemctl enable apache2
    SHELL
  end

  # MySQL VM
  config.vm.define "mysql" do |mysql|
    mysql.vm.box = "ubuntu/jammy64"
    mysql.vm.network "private_network", ip: "192.168.56.102"
    mysql.vm.provision "shell", inline: <<-SHELL
      sudo apt update
      sudo apt install -y mysql-server
      sudo systemctl enable mysql
    SHELL
  end
end
