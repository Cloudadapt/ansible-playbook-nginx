# ansible-playbook-nginx
install Wordpress on ubuntu ec2 instance using Nginx instead of apache by using Ansbile playbook



Make sure to replace the placeholders (`your_ec2_instance`, `your_mysql_root_password`, `your_wordpress_db_name`, `your_wordpress_db_user`, `your_wordpress_db_password`, and `your_domain_name`) with your actual values.

To execute the playbook, save it in a file (e.g., `wordpress.yml`) and run the following command:

ansible-playbook -i your_inventory_file wordpress.yml


Replace `your_inventory_file` with the path to your Ansible inventory file or specify the target host directly in the playbook by replacing `your_ec2_instance` with the IP address or hostname of your EC2 instance.

This playbook will install and configure Nginx, MySQL, PHP-FPM, and WordPress on your Ubuntu EC2 instance. It will also create the necessary database and user for WordPress. Finally, it will download the latest WordPress version, extract it, and configure the `wp-config.php` file.
