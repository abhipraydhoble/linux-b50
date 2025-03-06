
## Questions and Answers

### 1. A DevOps Engineer is troubleshooting a web application deployment. The deployment script fails with a "permission denied" error when trying to write to /var/www/html. As a Linux administrator, what would you suggest as the most appropriate immediate solution?

a) chmod 777 /var/www/html  
b) chown -R apache:apache /var/www/html (Assuming Apache is the webserver user)  
c) sudo su - and then run the deployment  
d) Reboot the server.  

**Answer:** b) chown -R apache:apache /var/www/html (Assuming Apache is the webserver user)

### 2. As an AWS Cloud Engineer, you're tasked with creating a script to automate the backup of a MySQL database running on an EC2 instance. What command is most suitable for creating a compressed database backup?

a) cp -r /var/lib/mysql /backup  
b) mysqldump -u root -p[password] [database_name] | gzip > /backup/db_backup.sql.gz  
c) tar -czvf /backup/db_backup.tar.gz /var/lib/mysql  
d) rsync -avz /var/lib/mysql /backup  

**Answer:** b) mysqldump -u root -p[password] [database_name] | gzip > /backup/db_backup.sql.gz

### 3. A System Administrator is investigating high CPU usage on a Linux server. Which command is the best starting point to identify the process consuming the most CPU?

a) netstat -anp  
b) df -h  
c) top  
d) ping google.com  

**Answer:** c) top

### 4. A DevOps Engineer is writing a shell script to automate the deployment of an application. They need to check if a specific file exists before proceeding. Which conditional statement is most appropriate?

a) if [ $file -exists ]  
b) if [ -f "$file" ]  
c) if ( test -e "$file" )  
d) if [[ -e $file ]]  

**Answer:** b) if [ -f "$file" ]

### 5. As an AWS Certified SysOps Administrator, you want to manage user permissions more efficiently in Linux. Which of the following is the recommended way to manage users with common access needs?

a) Assign individual permissions using chmod for each user.  
b) Create groups and add users to those groups, then manage permissions based on the group.  
c) Use Access Control Lists (ACLs) exclusively.  
d) Create a separate user account for each task.  

**Answer:** b) Create groups and add users to those groups, then manage permissions based on the group.

### 6. A Linux Administrator needs to find all files in a directory and its subdirectories that are larger than 10MB. Which command would they use?

a) find . -size +10M  
b) ls -lR | grep "10M"  
c) du -sh * | grep "10M"  
d) grep -r "10M" .  

**Answer:** a) find . -size +10M

### 7. A DevOps Engineer is tasked with automating the process of creating a new user account on a fleet of Linux servers. Which command is the standard utility for adding a new user?

a) adduser  
b) newuser  
c) usercreate  
d) mkuser  

**Answer:** a) adduser

### 8. An AWS Engineer needs to check the network configuration of an EC2 instance to ensure it's properly connected to the VPC. Which command would be most helpful for displaying network interfaces and their configurations?

a) netstat -rn  
b) ifconfig (or ip addr on newer systems)  
c) ps -ef  
d) free -m  

**Answer:** b) ifconfig (or ip addr on newer systems)

---


