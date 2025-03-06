
### Linux 

1. **A DevOps Engineer is troubleshooting a web application deployment. The deployment script fails with a "permission denied" error when trying to write to `/var/www/html`. What is the most appropriate immediate solution?**
   - **Answer:** `chown -R apache:apache /var/www/html` (Assuming Apache is the webserver user)

2. **A System Administrator is investigating high CPU usage on a Linux server. Which command is the best starting point to identify the process consuming the most CPU?**
   - **Answer:** `top`

3. **A Linux Administrator needs to find all files in a directory and its subdirectories that are larger than 10MB. Which command would they use?**
   - **Answer:** `find . -size +10M`

4. **A DevOps Engineer is writing a shell script to automate the deployment of an application. They need to check if a specific file exists before proceeding. Which conditional statement is most appropriate?**
   - **Answer:** `if [ -f "$file" ]`

5. **A Linux Administrator needs to find the processes that are listening on a specific port. What command is most appropriate?**
   - **Answer:** `netstat -tulnp | grep <port_number>`

6. **A DevOps Engineer wants to schedule a script to run every day at 3:00 AM. Which tool would they typically use?**
   - **Answer:** `cron`

7. **As a Linux Administrator, you need to list all files and directories, including hidden ones, in the current directory. Which command will achieve this?**
   - **Answer:** `ls -a`

8. **A Linux Administrator wants to count the number of lines in a file. Which command should they use?**
   - **Answer:** `wc -l`

9. **A DevOps Engineer needs to ensure that all commands executed by a specific user are logged for auditing purposes. Which configuration would be most appropriate?**
   - **Answer:** Enable process accounting using `acct` or `auditd`

### AWS & Cloud Engineering

10. **As an AWS Cloud Engineer, you're tasked with creating a script to automate the backup of a MySQL database running on an EC2 instance. What command is most suitable for creating a compressed database backup?**
    - **Answer:** `mysqldump -u root -p[password] [database_name] | gzip > /backup/db_backup.sql.gz`

11. **An AWS Solutions Architect needs to configure a web server to automatically start after a system reboot. Which of the following is the best way to ensure this happens on a modern Linux system using systemd?**
    - **Answer:** `systemctl enable <service_name>`

12. **An AWS Engineer needs to check the network configuration of an EC2 instance to ensure it's properly connected to the VPC. Which command would be most helpful for displaying network interfaces and their configurations?**
    - **Answer:** `ifconfig` (or `ip addr` on newer systems)

13. **An AWS DevOps engineer wants to manage and store secrets like API keys and passwords. Which command will help achieve this?**
    - **Answer:** Use an AWS service like `AWS Secrets Manager`

14. **An AWS Engineer wants to mount an EBS volume to an EC2 instance. What is the first step they should take after attaching the volume to the instance?**
    - **Answer:** Format the EBS volume.

15. **An AWS Solutions Architect is configuring a Load Balancer and needs to ensure that traffic is only allowed from the Load Balancer to the EC2 instances. What security measure should be implemented?**
    - **Answer:** Use Security Groups to restrict inbound traffic to the EC2 instances to only the Load Balancer's Security Group.

### Networking & Security

16. **As an AWS DevOps Engineer, you're troubleshooting why your application cannot access a specific port on a remote server. What Linux utility would you use to verify if that port is listening on the remote server?**
    - **Answer:** `netstat` or `ss`

17. **A System Administrator wants to redirect all standard output and standard error of a command to a file named `output.log`. Which command accomplishes this?**
    - **Answer:** `command &> output.log`

18. **An AWS Cloud Support Engineer notices high network latency between two EC2 instances. Which command is most helpful for identifying the network path and potential bottlenecks?**
    - **Answer:** `traceroute` (or `tracepath`)

19. **As a Linux Admin, you want to see the last commands executed in the current shell session. Which command can you use?**
    - **Answer:** `history`

20. **A DevOps Engineer wants to find all occurrences of the word "ERROR" in all files within a directory. Which command should you use?**
    - **Answer:** `grep -r "ERROR" .`

---

