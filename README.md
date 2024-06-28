# Task
Static Website Deployment on AWS EC2 

# Objectives

Cloud Platform: Choose a cloud platform of your preference (AWS EC2, Azure, etc) to deploy your website.
Web Server: Select a web server software like NGINX or Apache to serve your static website content.
Website Preparation: Ensure your static website files (HTML, CSS, Javascript) are ready for deployment.
Server Configuration: Configure the chosen web server (NGINX or Apache) on your cloud instance to serve your website content and confirm that it is accessible through a public IP address or a domain name after deployment.

# Method

Cloud Platform: AWS \
OS: Ubuntu24 \
Size: 8Gb RAM \
Services: SSH, Apache2 \

# Solution

Navigate to the AWS EC2 dashboard
   create key pairs and security group(add your inbound rules)
   Launch instance 
   Add appropriate tags
   Choose AMI: Ubuntu 24
   Choose Security Group and launch instance

# Manual Website Setup

Navigate to Git Bash Terminal
   SSH into instance and run the following commands:
      sudo -i
      apt update
      apt install apache2 -y
      cd /var/www/html/
      vim index.html
      vim styles.css
      vim scripts.js
      systemctl restart apache2

# Get your IP address from your running instance and your static website is live
# Note: 
    Inbound rules is set to allow all traffic to Ipv4 and Ipv6 for the purpose of this project
    The .HTML, .css, .js files used can be found in this repository
    
  


   
