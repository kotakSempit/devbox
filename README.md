# DevBox

## Introduction
DevBox provides a PHP development environment using Vagrant and VirtualBox. The development VM created is built on Ubuntu with Apache, Nginx, PHP and MySQL. The VM can be configured to use different versions of Ubuntu, PHP and MySQL. It can also be configured to use either Apache or Nginx.


### Environtment Stack
* Ubuntu 16.04.04 LTS
* Apache 2.4.33
* PHP 7.2.9
* MySQL 5.7.22

### Required PHP Extensions (Installed)
* OpenSSL PHP Extension
* PDO PHP Extension
* Mbstring PHP Extension
* Tokenizer PHP Extension
* XML PHP Extension
* Ctype PHP Extension
* JSON PHP Extension

### Directory Structure
    .
    ├── code                   # Root folder for web application
    │   └── index.php                     
    ├── scripts                # Vagrant provisioning scripts
    ├── config.yaml            # Vagrant configuration file
    ├── Vagrantfile            
    └── README.md

` code ` folder is synced with ` /home/vagrant ` folder in VM.

### Site Informations
Website can be accessed at http://localhost:8000
Virtual host ` site.test ` is available, but need to add to the url in our machine ` host ` file first.

### Database Credentials
* MySQL Host: 127.0.0.1
* MYSQL Server Port: 3306
* Username: root
* Password: secret

### Database Access Via MySQL Workbench
* Connection Method: Standard TCIP/IP over SSH
* SSH Hostname: 127.0.0.1:2222
* SSH Username: vagrant
* SSH Password: vagrant
