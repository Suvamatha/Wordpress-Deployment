# WordPress and MySQL Deployment with Vagrant
This repository contains the setup for deploying WordPress and MySQL using Vagrant, Ubuntu, and Oracle VirtualBox. It provides a simple way to provision two virtual machines: one for WordPress and the other for MySQL.

## Prerequisites
Ensure you have the following tools installed on your machine:

. Vagrant
. Oracle VirtualBox
. Git (for cloning this repository)
. Project Structure
. bash
. Copy code
.
--

## Project Structure
├── Vagrantfile               # Vagrant configuration for the two VMs
├── wordpress/                # WordPress VM configuration
│   ├── setup.sh              # Provisioning script for WordPress
│   └── wp-config.php         # WordPress configuration file
├── mysql/                    # MySQL VM configuration
│   └── setup.sh              # Provisioning script for MySQL
└── README.md                 # Project documentation
Getting Started
Follow these steps to set up the project and deploy WordPress:

1. Clone the Repository
bash
Copy code
[git clone] (https://github.com/your-username/Wordpress-Deployment.git)
cd Wordpress-Deployment
2. Launch the Virtual Machines
Start both virtual machines using Vagrant:

bash
Copy code
vagrant up
3. Access the WordPress Site
Once the VMs are running:

Open your browser and navigate to the WordPress VM's IP address. For example: http://<wordpress-vm-ip>
4. Database Configuration
The MySQL VM is pre-configured with:

Database Name: wordpress
User: wp_user
Password: strong_password
Update the wp-config.php file with the correct database connection details.

Customization
WordPress VM:
Modify wordpress/setup.sh for additional custom configurations.
MySQL VM:
Modify mysql/setup.sh to change the database setup or user permissions.
Contributing
Contributions are welcome! Feel free to open issues or submit pull requests to improve this project.