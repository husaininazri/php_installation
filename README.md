# php_installation
# apache_installation on Linux Server

How To Install Linux, Apache, MySQL, PHP (LAMP) stack on Ubuntu 18.04

### Prerequisites

* Link 
  ```sh
    https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-ubuntu-18-04
  ```

* Let’s begin by updating the local package index to reflect the latest upstream changes:
  ```sh
  sudo apt update
  sudo apt install apache2
  ```

* List the ufw application profiles by typing:
  ```sh
  sudo ufw app list
    
    Output
    Available applications:
      Apache
      Apache Full
      Apache Secure
      OpenSSH
  ```

* Since we haven’t configured SSL for our server yet in this guide, we will only need to allow traffic on port 80:
  ```sh
  sudo ufw allow 'Apache'
  sudo ufw status
  ```
