# Magento 2 Installation and Configuration with MYSQL 8, ELASTICSEARCH, REDIS, PHPMYADMIN and VARNISH

## Prerequisites
1. Launch an instance of Debian 11.
2. Install the following components:
   - PHP 8.1
   - MySQL 8
   - NGINX
   - Elasticsearch
   - Redis
   - Phpmyadmin
   - Varnish

## Installation Steps
1. Install Magento 2 via Composer with Sample Data and Elasticsearch.
   
2. Install Redis-Server and configure Magento to use Redis for cache and sessions.

3. Change ownership of all files to user "test" and group "test-grp".

4. Configure NGINX to run as user "test-grp".
   - Create a PHP-FPM pool that runs as user "test" and group "test-grp".
   - Use this PHP-FPM pool in your NGINX vhost.

5. Configure PHPMyAdmin with Docker.

6. Redirect HTTP to HTTPS in NGINX.
   - Set up all store URLs to HTTPS with a self-signed certificate.

7. Install Varnish and configure it with Magento.

## Repository Structure
 - **php_script**: Contains scripts for automation of php installation.
 - **/nginx-conf**: Configuration file of magento server block for NGINX.

## Usage
1. Clone this repository.
2. Run setup script to automate php installation and  manually configure as per instructions in the installation_commands.

## Contributing
Please feel free to contribute by opening issues or pull requests for any improvements or enhancements.

## License
This project is licensed under the [MIT License](LICENSE).
