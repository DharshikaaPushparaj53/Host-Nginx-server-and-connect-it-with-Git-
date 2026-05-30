# Host-Nginx-server-and-connect-it-with-Git-
Hosting an app in an Nginx web server and connecting it to a Git version control system

1. Create a VM in the AWS platform
   
2. Update and upgrade the Instance
   
     sudo apt update -y
   
     sudo apt upgrade -y

3. Install the Nginx server on the virtual machine instance

     apt install nginx -y

     systemctl start nginx

     systemctl enable nginx

     systemctl status nginx

4. Test Nginx

     http://3.15.171.16

Public IP address of your instance. (Welcome to nginx page will appear)

5. Create your HTML application

     cd /var/www/html

     ls

     index.nginx-debian.html

     rm index.nginx-debian.html

6. Create an HTML file

     vim index.html

     

     
