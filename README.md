# DevOps-Project001
First project from the guided Darey.io DevOps Engineer Scholarship 

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
  




