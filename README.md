# 2-tier-with-docker
a project on docker using wordpress & mysql

# 🚀 Learning Docker – 2-Tier Architecture with WordPress & MySQL 🐳

Excited to share my hands-on learning experience with **Docker**!  
I worked on a **2-tier architecture** setup using:

- 🖥️ **WordPress** as the frontend
- 🗄️ **MySQL** as the backend

All services are containerized using Docker! 🐋

## 🔧 Steps Followed:

1. **Pulled Docker Images**
   - `wordpress`
   - `mysql`

2. **Created a MySQL Container** with environment variables:
   ```env
   MYSQL_ROOT_PASSWORD=your_root_password
   MYSQL_DATABASE=your_db_name
   
Set up WordPress Container linked to the MySQL container:
env
Copy
Edit

WORDPRESS_DB_HOST=mysql_container_name:3306
WORDPRESS_DB_USER=root
WORDPRESS_DB_PASSWORD=your_root_password
WORDPRESS_DB_NAME=your_db_name

🧠 After Container Setup:
Accessed WordPress via browser using exposed IP or localhost:port

Completed WordPress installation 🎉

Added a sample post & comment to test data flow

🔍 Verified MySQL Data via Docker:
bash
Copy
Edit
docker exec -it <mysql_container_id> /bin/bash
mysql -u root -p
SHOW DATABASES;
USE your_db_name;
SHOW TABLES;

💡 Key Takeaways
Understood how to set up multi-container applications using Docker

Learned about inter-container communication

Experienced practical implementation of a 2-tier architecture

📌 Tags
#Docker #WordPress #MySQL #DevOps #LearningByDoing #Containerization #2TierArchitecture #CloudJourney
