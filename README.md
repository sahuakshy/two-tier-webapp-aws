🚀 Two-Tier Web Architecture on AWS with Joomla
Deploy a Two-Tier Web Architecture using AWS EC2, RDS, and Joomla CMS. This setup separates the web layer and database layer for better scalability and security.

🏗 Architecture Overview
1- Web Layer (EC2): Hosts Joomla website
2- Database Layer (RDS): MySQL/MariaDB database
3- Flow: Joomla on EC2 connects to RDS for data storage

⚡ Deployment Steps
1️⃣ Create RDS Database:-
* Go to AWS Console → RDS → Create Database
* Choose MySQL/MariaDB, set username & password
* Configure VPC Security Group (allow EC2 access)

2️⃣ Launch EC2 Instance
* EC2 → Launch Instance → Amazon Linux 
* Open HTTP (80) & SSH (22) ports in Security Groups

3️⃣ Install Joomla on EC2
4️⃣ Connect Joomla to RDS
* During Joomla setup, enter:
* Database Type: MySQLi
* Host Name: RDS endpoint
* Username & Password: RDS credentials
* Database Name: RDS database

5️⃣ Verify Deployment
*  Access your Joomla site via EC2 public IP
*  Ensure all data is stored in RDS
