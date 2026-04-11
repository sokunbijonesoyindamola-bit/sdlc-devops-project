# Linux Project 6 (LEMP Stack)

## Step 1: Update Package Repository

Command used:  
sudo apt update  

### Output  
![Step 1](Images/li6-step1.png)

---

## Step 2: Install Nginx

Command used:  
sudo apt install nginx  

### Output  
![Step 2](Images/li6-step2.png)

---

## Step 3: Check Available UFW Profiles

Command used:  
sudo ufw app list  

### Output  
![Step 3](Images/li6-step3.png)

---

## Step 4: Allow Nginx HTTP Through Firewall

Command used:  
sudo ufw allow 'Nginx HTTP'  

### Output  
![Step 4](Images/li6-step4.png)

---

## Step 5: Verify Firewall Status

Command used:  
sudo ufw status  

### Output  
![Step 5](Images/li6-step5.png)

---

## Step 6: Check Server IP Address

Command used:  
ip addr show enp0s3  

### Output  
![Step 6](Images/li6-step6.png)

---

## Step 7: Test Nginx in Browser

URL used:  
http://localhost:8080  

### Output  
![Step 7](Images/li6-step7.png)

---

## Step 8: Install MySQL Server

Command used:  
sudo apt install mysql-server  

### Output  
![Step 8](Images/li6-step8.png)

---

## Step 9: Secure MySQL Installation

Command used:  
sudo mysql_secure_installation  

### Output  
![Step 9](Images/li6-step9.png)

---

## Step 10: Log into MySQL

Command used:  
sudo mysql  

### Output  
![Step 10](Images/li6-step10.png)

---

## Step 11: Install PHP and Required Modules

Command used:  
sudo apt install php-fpm php-mysql  

### Output  
![Step 11](Images/li6-step11.png)

---

## Step 12: Create Project Directory

Command used:  
sudo mkdir /var/www/your_domain  

### Output  
![Step 12](Images/li6-step12.png)

---

## Step 13: Set Directory Ownership

Command used:  
sudo chown -R $USER:$USER /var/www/your_domain  

### Output  
![Step 13](Images/li6-step13.png)

---

## Step 14: Create Nginx Configuration File

Command used:  
sudo nano /etc/nginx/sites-available/your_domain  

### Output  
![Step 14](Images/li6-step14.png)

---

## Step 15: Enable Configuration

Command used:  
sudo ln -s /etc/nginx/sites-available/your_domain /etc/nginx/sites-enabled/  

### Output  
![Step 15](Images/li6-step15.png)

---

## Step 16: Disable Default Configuration

Command used:  
sudo unlink /etc/nginx/sites-enabled/default  

### Output  
![Step 16](Images/li6-step16.png)

---

## Step 17: Test Nginx Configuration

Command used:  
sudo nginx -t  

### Output  
![Step 17](Images/li6-step17.png)

---

## Step 18: Reload Nginx

Command used:  
sudo systemctl reload nginx  

### Output  
![Step 18](Images/li6-step18.png)

---

## Step 19: Create PHP Info File

Command used:  
nano /var/www/your_domain/info.php  

### Output  
![Step 19](Images/li6-step19.png)

---

## Step 20: Access PHP Page in Browser

URL used:  
http://localhost:8080/info.php  

### Output  
![Step 20](Images/li6-step20.png)