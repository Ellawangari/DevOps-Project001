# DevOps-Project001
First project from the guided [title](https://www.darey.io) DevOps Engineer Scholarship 

**Project Implementation**
Technology Stack used was **LAMP**( Linux Apache MYSQL PHP)

**Step 1: Creating an AWS instance & Connecting to it using Mobaxterm**
- Created an Amazon account and provisioned an Ubuntu Server 20.04 LTS (HVM), SSD Volume Type EC2 Instance with a free tier option.
 ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/amazon%20instance%201.PNG)
- Downloaded my pem file to access my  AWS Ubuntu server using Mobaxterm on my windows pc.
- Made the download folder as the persistent home directory since that's where my pem file was located.
 ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/mobaxterm1.PNG)
- Added new inbound rules to connect to the instance using SSH.
 ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/aws%204.PNG)
- Once the inbound rules were all set I was now able to connect to my instance using the SSH on Mobaxterm.
 ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/mobaxterm2.PNG)
 
**Step 2: Downloading Oracle virtual box , installing Ubuntu Os to practice Linux commands**
- Downloaded Oracle virtual box on my windows pc and installed Ubuntu Os.
  ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/ubuntu1.PNG)
- Logged in to Ubuntu and opened the terminal to practice a few Linux commands.
   - ls command to list files in my home directory
   - Created a  file called Learning_Linux on the Desktop added commands learned to it and navigated to it.
    ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/ubuntu4.PNG)
   - cat command to read the contents of the file.
        ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/ubuntu5.PNG)
   -Practiced on a lot more commands.
   
   **Step 3: Installing Apache in my AWS instance and updating firewall**
   - Connected to the AWS instance on Mobaxterm and installed Apache  and runned the following command to verify that apache service in our server.
       `sudo systemctl status apache2`
      ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/mobaxterm3.PNG)
   - Added another  http inbound rule  to my AWS instance which was to open port 80.
      ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/aws%204.PNG)
      
     **Step 4: Installing MYSQL **
  - Connected to the AWS instance on Mobaxterm and installed MYSQL  and runned the following command to test if i can log in to MYSQL console.
   ` sudo apt install mysql-server`
    ` sudo mysql`
     ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/mobaxterm4.PNG)
   -Which was successful and ran the following command to exit MYSQL command.
      ` mysql> exit`
    **Step 4: Installing PHP **
  - Connected to the AWS instance on Mobaxterm and installed PHP  and runned the following command to check the version installed.
   ` sudo apt install php libapache2-mod-php php-mysql`  ` php -v`
       ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/mobaxterm5.PNG)
  - Created a Virtual host for my website using Apache
    -Created a directory for projectlamp using the mkdir command
    -Assigned ownership of the directory to the current system user
    -Then created and opened a new configuration file in Apache’s sites-available directory and added the followin details.
     ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/mobaxterm6.PNG)
    -Enabled PHP on the website by changing the default DirectoryIndex settings on Apache to start with index.php instead of index.html
      ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/mobaxterm7.PNG)
    -Created an index.php inside the custom web root folder and opened the file to add the following code.
     `<?php
phpinfo();`
       ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/mobaxterm8.PNG)
     - Reloaded my webite on the browser and the php page loaded successfully.
     ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/phppage.PNG)
     - Finally removed the file as it contained sensitive information using the following command  `sudo rm /var/www/projectlamp/index.php `
     Reloaded the site to confirm the file was removed successfully.
        ![alt text](https://github.com/Ellawangari/DevOps-Project001/blob/main/Images/phppage2.PNG)

**
End for DevOps Project 1**

To try this project  [title](https://www.darey.io) have a free trial to which you can practice this project.
