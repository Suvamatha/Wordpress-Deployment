# WordPress and MySQL Deployment with Vagrant

This repository provides a setup to deploy WordPress and MySQL using [Vagrant](https://www.vagrantup.com/), [Ubuntu](https://ubuntu.com/), and [Oracle VirtualBox](https://www.virtualbox.org/). It includes two virtual machines: one for hosting the WordPress application and the other for running the MySQL database.

## Project Structure

```,plaintext
├── Vagrantfile               # Vagrant configuration for the two VMs
├── wordpress/                # WordPress VM configuration
│   ├── setup.sh              # Provisioning script for WordPress
│   └── wp-config.php         # WordPress configuration file
├── mysql/                    # MySQL VM configuration
│   └── setup.sh              # Provisioning script for MySQL
└── README.md                 # Project documentation


```
## 1.Getting Started
Follow these steps to set up the project and deploy WordPress:
[git clone] (https://github.com/Suvamatha/Wordpress-Deployment.git)

##  2.Launch the Virtual Machines
Start both virtual machines using Vagrant:
(vagrant up)

## 3. Access the WordPress Site
Once the VMs are running:

Open your browser and navigate to the WordPress VM's IP address. For example:
plaintext

(http://<wordpress-vm-ip>)

## 4. Database Configuration
The MySQL VM is pre-configured with:

(- Database Name: wordpress
- User: wp_user
- Password: strong_password
Update the wp-config.php file with the correct database connection details.)

