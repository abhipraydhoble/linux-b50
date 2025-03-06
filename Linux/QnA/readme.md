Questions:

Question: A DevOps Engineer is troubleshooting a web application deployment. The deployment script fails with a "permission denied" error when trying to write to /var/www/html. As a Linux administrator, what would you suggest as the most appropriate immediate solution?

a) chmod 777 /var/www/html b) chown -R apache:apache /var/www/html (Assuming Apache is the webserver user) c) sudo su - and then run the deployment d) Reboot the server.

Answer: b) chown -R apache:apache /var/www/html (Assuming Apache is the webserver user)

Question: As an AWS Cloud Engineer, you're tasked with creating a script to automate the backup of a MySQL database running on an EC2 instance. What command is most suitable for creating a compressed database backup?

a) cp -r /var/lib/mysql /backup b) mysqldump -u root -p[password] [database_name] | gzip > /backup/db_backup.sql.gz c) tar -czvf /backup/db_backup.tar.gz /var/lib/mysql d) rsync -avz /var/lib/mysql /backup

Answer: b) mysqldump -u root -p[password] [database_name] | gzip > /backup/db_backup.sql.gz

Question: A System Administrator is investigating high CPU usage on a Linux server. Which command is the best starting point to identify the process consuming the most CPU?

a) netstat -anp b) df -h c) top d) ping google.com

Answer: c) top

Question: A DevOps Engineer is writing a shell script to automate the deployment of an application. They need to check if a specific file exists before proceeding. Which conditional statement is most appropriate?

a) if [ $file -exists ] b) if [ -f "$file" ] c) if ( test -e "$file" ) d) if [[ -e $file ]]

Answer: b) if [ -f "$file" ]

Question: As an AWS Certified SysOps Administrator, you want to manage user permissions more efficiently in Linux. Which of the following is the recommended way to manage users with common access needs?

a) Assign individual permissions using chmod for each user. b) Create groups and add users to those groups, then manage permissions based on the group. c) Use Access Control Lists (ACLs) exclusively. d) Create a separate user account for each task.

Answer: b) Create groups and add users to those groups, then manage permissions based on the group.

Question: A Linux Administrator needs to find all files in a directory and its subdirectories that are larger than 10MB. Which command would they use?

a) find . -size +10M b) ls -lR | grep "10M" c) du -sh * | grep "10M" d) grep -r "10M" .

Answer: a) find . -size +10M

Question: A DevOps Engineer is tasked with automating the process of creating a new user account on a fleet of Linux servers. Which command is the standard utility for adding a new user?

a) adduser b) newuser c) usercreate d) mkuser

Answer: a) adduser

Question: An AWS Engineer needs to check the network configuration of an EC2 instance to ensure it's properly connected to the VPC. Which command would be most helpful for displaying network interfaces and their configurations?

a) netstat -rn b) ifconfig (or ip addr on newer systems) c) ps -ef d) free -m

Answer: b) ifconfig (or ip addr on newer systems)

Question: A System Administrator wants to redirect all standard output and standard error of a command to a file named output.log. Which command accomplishes this?

a) command > output.log b) command 2> output.log c) command &> output.log d) command | tee output.log

Answer: c) command &> output.log

Question: A DevOps Engineer is using SSH to connect to a remote server, but keeps getting disconnected. What command can they use to maintain the SSH session even if the local terminal closes?

a) ssh -N user@host b) ssh user@host & c) nohup ssh user@host & d) screen ssh user@host (or tmux)

Answer: d) screen ssh user@host (or tmux)

Question: An AWS Solutions Architect needs to configure a web server to automatically start after a system reboot. Which of the following is the best way to ensure this happens on a modern Linux system using systemd?

a) Edit the /etc/rc.local file. b) Use chkconfig to enable the service. c) Use systemctl enable <service_name> d) Create a cron job that runs on reboot.

Answer: c) Use systemctl enable <service_name>

Question: A Linux Administrator wants to view the last 10 lines of a log file. Which command should they use?

a) head -n 10 logfile.txt b) tail -n 10 logfile.txt c) cat logfile.txt | head -n 10 d) more logfile.txt

Answer: b) tail -n 10 logfile.txt

Question: A DevOps engineer is automating application deployment and needs to transfer a file securely to a remote Linux server. Which command is most appropriate?

a) ftp b) scp c) telnet d) wget

Answer: b) scp

Question: As an AWS DevOps Engineer, you're troubleshooting why your application cannot access a specific port on a remote server. What Linux utility would you use to verify if that port is listening on the remote server?

a) ping b) traceroute c) netstat or ss d) arp

Answer: c) netstat or ss

Question: A system administrator needs to find the processes that are listening on a specific port. What command is most appropriate?

a) ps -ef | grep <port_number> b) netstat -tulnp | grep <port_number> c) kill -9 <port_number> d) df -h

Answer: b) netstat -tulnp | grep <port_number>

Question: As an AWS Cloud Support Engineer, you encounter a situation where a process is consuming a lot of I/O resources on a Linux server. Which command is most suitable for identifying the process?

a) top b) iotop c) free -m d) ps -aux

Answer: b) iotop

Question: A DevOps engineer is writing a script to automate the creation of a directory. They want to ensure the script doesn't fail if the directory already exists. Which command should they use?

a) mkdir directory_name b) mkdir -p directory_name c) mkdir -f directory_name d) touch directory_name

Answer: b) mkdir -p directory_name

Question: As a Linux System Admin, you have a compressed file named "archive.tar.gz". What command would you use to extract its contents?

a) tar -xf archive.tar.gz b) tar -cvf archive.tar.gz c) tar -zxvf archive.tar.gz d) gzip -d archive.tar.gz

Answer: c) tar -zxvf archive.tar.gz

Question: As an AWS Engineer, you need to view the contents of a text file without opening it in an editor. You only need to view the file contents once. Which command is the most efficient?

a) vi file.txt b) nano file.txt c) cat file.txt d) echo file.txt

Answer: c) cat file.txt

Question: As a DevOps Engineer, you want to find all occurrences of the word "ERROR" in all files within a directory. Which command should you use?

a) ls -l | grep ERROR b) find . -name "*ERROR*" c) grep -r "ERROR" . d) locate ERROR

Answer: c) grep -r "ERROR" .

Question: A Linux Administrator is trying to understand the system boot process. Which file typically contains the boot messages?

a) /var/log/syslog b) /var/log/boot.log c) /var/log/messages d) /proc/cmdline

Answer: b) /var/log/boot.log

Question: An AWS DevOps engineer wants to manage and store secrets like API keys and passwords. Which command will help you achieve this?

a) export API_KEY='your_api_key' b) Use an AWS service like AWS Secrets Manager c) echo "API_KEY=your_api_key" >> .bashrc d) Store the keys in a plain text file in /opt/

Answer: b) Use an AWS service like AWS Secrets Manager

Question: A system administrator needs to change the ownership of a file named data.txt to a user named "john". Which command should they use?

a) chmod john data.txt b) chown john data.txt c) useradd john data.txt d) passwd john data.txt

Answer: b) chown john data.txt

Question: You are a DevOps Engineer and you need to find the IP address of a domain name. Which command can you use?

a) ifconfig b) ping c) nslookup d) traceroute

Answer: c) nslookup

Question: As a Linux administrator, you need to list all files and directories, including hidden ones, in the current directory. Which command will achieve this?

a) ls b) ls -a c) ls -l d) ls -R

Answer: b) ls -a

Question: A DevOps Engineer wants to schedule a script to run every day at 3:00 AM. Which tool would they typically use?

a) at b) batch c) cron d) watch

Answer: c) cron

Question: As an AWS Engineer, you need to identify the process ID (PID) of a running process named "my_app". What command would be most appropriate?

a) ps -ef | grep my_app b) killall my_app c) top d) df -h

Answer: a) ps -ef | grep my_app

Question: A Linux Administrator needs to terminate a process with a specific PID. Which command should they use?

a) kill b) stop c) halt d) shutdown

Answer: a) kill

Question: A DevOps Engineer is trying to figure out which packages are installed on a Debian-based system. Which command is most suitable?

a) rpm -qa b) yum list installed c) dpkg -l d) pkg list

Answer: c) dpkg -l

Question: As an AWS Engineer, you want to monitor the real-time usage of disk space on your EC2 instance. Which command would be most useful?

a) free -m b) df -h c) du -sh d) top

Answer: b) df -h

Question: A System Administrator needs to change the permissions of a script so that only the owner can execute it. What chmod command should they use?

a) chmod 777 script.sh b) chmod 755 script.sh c) chmod 700 script.sh d) chmod 644 script.sh

Answer: c) chmod 700 script.sh

Question: As a DevOps Engineer, you're writing a script that needs to get the output of a command and store it in a variable. How would you achieve this in bash?

a) variable = command b) variable := command c) variable=$(command) d) variable=[command]

Answer: c) variable=$(command)

Question: You are an AWS Certified SysOps Administrator troubleshooting a networking issue. You suspect that the firewall is blocking traffic. Which command can help you view the active firewall rules on a Linux system using iptables?

a) iptables -L b) firewall-cmd --list-all (if using firewalld) c) ufw status (if using ufw) d) All of the above, depending on the firewall configuration.

Answer: d) All of the above, depending on the firewall configuration.

Question: A DevOps Engineer needs to find all files modified in the last 24 hours. Which find command is most suitable?

a) find . -mtime 1 b) find . -mmin 1440 c) find . -atime 1 d) find . -ctime 1

Answer: a) find . -mtime 1

Question: As an AWS Cloud Engineer, you need to determine the fully qualified domain name (FQDN) of your EC2 instance. Which command is most likely to provide this information directly?

a) hostname b) hostname -f c) uname -n d) ip addr

Answer: b) hostname -f

Question: You are a Linux System Admin and you want to switch to another user account temporarily. What command should you use?

a) su b) sudo c) passwd d) useradd

Answer: a) su

Question: A DevOps Engineer is using sed to replace all occurrences of "old_string" with "new_string" in a file named config.txt. Which command would be most appropriate?

a) sed 's/old_string/new_string/g' config.txt b) sed 's/old_string/new_string/' config.txt c) sed 's/old_string/new_string' config.txt d) sed -i 's/old_string/new_string/g' config.txt

Answer: d) sed -i 's/old_string/new_string/g' config.txt

Question: An AWS Engineer wants to mount an EBS volume to an EC2 instance. What is the first step they should take after attaching the volume to the instance?

a) Format the EBS volume. b) Create a mount point directory. c) Mount the volume to the mount point directory. d) Partition the EBS Volume.

Answer: a) Format the EBS volume.

Question: A Linux Administrator wants to count the number of lines in a file. Which command should they use?

a) wc -w b) wc -l c) wc -c d) wc -m

Answer: b) wc -l

Question: As a DevOps Engineer, which command would you use to display the routing table on a Linux system?

a) ifconfig b) netstat -rn c) route -n d) Both b and c.

Answer: d) Both b and c.

Question: As an AWS Engineer, you are tasked with monitoring the memory usage of an EC2 instance. Which command gives you a real-time view of memory usage?

a) df -h b) top c) lsblk d) netstat -an

Answer: b) top

Question: A Linux Administrator wants to know the location of the executable for a particular command. Which command helps determine this?

a) whereis b) which c) locate d) find

Answer: b) which

Question: As a DevOps engineer you have a folder named myproject in your root directory. How would you use tar to create a compressed archive myproject.tar.gz of this folder?

a) tar -cvzf myproject.tar.gz myproject b) tar -xvzf myproject.tar.gz myproject c) tar -cvf myproject myproject.tar.gz d) tar -xvzf myproject

Answer: a) tar -cvzf myproject.tar.gz myproject

Question: An AWS Solutions Architect is configuring a Load Balancer and needs to ensure that traffic is only allowed from the Load Balancer to the EC2 instances. What security measure should be implemented?

a) Open port 80 and 443 to the world on the EC2 instances. b) Use Security Groups to restrict inbound traffic to the EC2 instances to only the Load Balancer's Security Group. c) Disable the firewall on the EC2 instances. d) Use IAM roles to grant access to the Load Balancer.

Answer: b) Use Security Groups to restrict inbound traffic to the EC2 instances to only the Load Balancer's Security Group.

Question: A DevOps Engineer is writing a Bash script and needs to perform a different action based on whether a file is a regular file or a directory. Which test operator can be used to check if a path is a regular file?

a) -d b) -f c) -x d) -w

Answer: b) -f

Question: As a Linux Admin, you want to see the last commands executed in the current shell session. Which command can you use?

a) history b) last c) who d) uptime

Answer: a) history

Question: An AWS Cloud Support Engineer notices high network latency between two EC2 instances. Which command is most helpful for identifying the network path and potential bottlenecks?

a) ping b) traceroute (or tracepath) c) netstat d) dig

Answer: b) traceroute (or tracepath)

Question: As a Linux Administrator, you need to find all files that have been accessed within the last 7 days. What command will achieve this?

a) find . -atime -7 b) find . -mtime -7 c) find . -ctime -7 d) find . -amin -7

Answer: a) find . -atime -7

Question: As a DevOps Engineer, you need to ensure that all commands executed by a specific user are logged for auditing purposes. Which configuration would be most appropriate?

a) Modify the user's .bashrc to include history command. b) Enable process accounting using acct or auditd. c) Force the user to use sudo for all commands. d) Create a cron job that runs ps -ef every minute.

Answer: b) Enable process accounting using acct or auditd.

Question: You are an AWS DevOps Engineer trying to determine the cause of a service outage. You suspect a recent change to a configuration file may be the problem. Which command would be most helpful in comparing the current configuration file to a previous version?

a) grep b) cat c) diff d) head

Answer: c) diff
