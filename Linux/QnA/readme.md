
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

Question 1: You need to find all files in the /home/user1 directory that are larger than 10MB. Which command is the most efficient way to do this?

a) ls -l /home/user1 | grep "10485760"
b) find /home/user1 -size +10M
c) for i in /home/user1/*; do du -h $i | grep M; done
d) locate /home/user1 | du -h | grep M

Answer: b) find /home/user1 -size +10M

Question 2: A user reports that their application is running very slowly. You suspect a memory leak. Which command would you use to identify the process consuming the most memory?

a) ps aux | sort -nrk 4,4
b) top
c) free -m
d) df -h

Answer: b) top

Question 3: You need to schedule a script to run every day at 3:00 AM. Which method is the most appropriate?

a) Edit the /etc/rc.local file.
b) Create a systemd service.
c) Use the at command.
d) Use crontab -e.

Answer: d) crontab -e

Question 4: Your server's root partition is running out of space. You need to quickly identify the largest directories under /. Which command will help you accomplish this?

a) du -sh / | sort -hr
b) df -h /
c) ls -l / | sort -nk 5,5
d) find / -type d

Answer: a) du -sh / | sort -hr

Question 5: You want to grant a user 'john' the ability to execute the reboot command without needing to provide a password. What is the best approach?

a) Add john to the sudoers file using visudo and granting permission to run /sbin/reboot.
b) Change the permissions of /sbin/reboot to 777.
c) Create an alias for reboot that doesn't require a password.
d) Directly edit /etc/passwd to remove the password requirement for john.

Answer: a) Add john to the sudoers file using visudo and granting permission to run /sbin/reboot.

Question 6: You need to change the ownership of all files and directories in /var/www/html to the user webmaster and the group www-data. Which command should you use?

a) chown -R webmaster:www-data /var/www/html
b) chmod -R webmaster:www-data /var/www/html
c) useradd webmaster:www-data /var/www/html
d) groupadd webmaster:www-data /var/www/html

Answer: a) chown -R webmaster:www-data /var/www/html

Question 7: A service is failing to start. You want to examine the service's logs to understand the reason for the failure. The service name is "my_app". Where would you typically look for the logs?

a) /var/log/my_app.log or using journalctl -u my_app
b) /etc/my_app/logs
c) /root/my_app/logs
d) /opt/my_app/logs

Answer: a) /var/log/my_app.log or using journalctl -u my_app

Question 8: You need to create a new user account named 'developer' with the user ID 1005 and add them to the group 'developers'. Which command would you use?

a) useradd -u 1005 -g developers developer
b) adduser -u 1005 -g developers developer
c) newuser -u 1005 -g developers developer
d) createuser -u 1005 -g developers developer

Answer: a) useradd -u 1005 -g developers developer

Question 9: You want to create a symbolic link named latest pointing to the file version-1.2.3.txt in the current directory. Which command achieves this?

a) cp version-1.2.3.txt latest
b) mv version-1.2.3.txt latest
c) ln -s version-1.2.3.txt latest
d) touch latest version-1.2.3.txt

Answer: c) ln -s version-1.2.3.txt latest

Question 10: You've accidentally deleted an important file. You have backups enabled. What's the first step to restore the file?

a) Immediately shut down the server to prevent further data loss.
b) Locate the backup medium and use the appropriate tool (e.g., tar, rsync) to restore the file.
c) Run fsck on the filesystem.
d) Reinstall the operating system.

Answer: b) Locate the backup medium and use the appropriate tool (e.g., tar, rsync) to restore the file.

