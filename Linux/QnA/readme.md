
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

### 9. You need to quickly view the contents of a large log file, but only the last 10 lines are relevant. Which command is the most efficient for this?

a) cat logfile.txt  
b) more logfile.txt  
c) tail logfile.txt  
d) head logfile.txt  

**Answer:** c) tail logfile.txt

### 10. A user reports they can't execute a script called myscript.sh. The script exists and the user has read permissions. What's the most likely problem?

a) The script is corrupted.  
b) The script doesn't have execute permissions.  
c) The user doesn't have write permissions to the directory.  
d) The user's home directory is full.  

**Answer:** b) The script doesn't have execute permissions.

### 11. You want to find all files in the current directory (and its subdirectories) that end with the .txt extension. Which command will accomplish this?

a) ls *.txt  
b) find . -name "*.txt"  
c) grep .txt  
d) locate *.txt  

**Answer:** b) find . -name "*.txt"

### 12. Your system is running slowly. You suspect a specific process is consuming excessive CPU. Which command will help you identify the culprit?

a) df -h  
b) ps -aux  
c) free -m  
d) ping google.com  

**Answer:** b) ps -aux

### 13. You need to copy a file named document.pdf from your local machine to a remote server using SSH. The remote server's username is user1 and the IP address is 192.168.1.100. The destination directory on the remote server is /home/user1/documents. Which command should you use?

a) cp document.pdf user1@192.168.1.100:/home/user1/documents  
b) scp document.pdf user1@192.168.1.100:/home/user1/documents  
c) mv document.pdf user1@192.168.1.100:/home/user1/documents  
d) ssh user1@192.168.1.100 "cp document.pdf /home/user1/documents"  

**Answer:** b) scp document.pdf user1@192.168.1.100:/home/user1/documents

### 14. You need to find out what IP address is currently assigned to your network interface eth0. Which command is most likely to provide this information?

a) ping google.com  
b) hostname  
c) ifconfig eth0 or ip addr show eth0  
d) netstat -rn  

**Answer:** c) ifconfig eth0 or ip addr show eth0

### 15. A process is consuming a lot of resources and you need to stop it. You know the process ID (PID) is 1234. Which command should you use?

a) kill 1234  
b) stop 1234  
c) remove 1234  
d) delete 1234  

**Answer:** a) kill 1234

