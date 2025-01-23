# Types of Users in Linux

## 1. $${\color{red} \textbf {Root User}}$$

- The root user is the superuser in Linux with unrestricted access to the entire system.
- They can perform any administrative task, including creating and deleting users, modifying files, and configuring the system.
- user id is 0

**Common Commands for Root User:**
```bash
# Switch to root user
sudo -i
````

**Execute a command as root**
````
sudo <command>
````

## 2. $${\color{blue} \textbf {System Users}}$$
- These are service accounts created by the system to manage and run specific processes or services.
- Do not have login shells by default.
- Limited privileges, ensuring security for system services.
- user id ranges from 1 - 999

  
## 3. $${\color{green} \textbf {Local User}}$$
- These are standard users created for daily tasks and operations.
- Each user has their own home directory (e.g., /home/username) and specific permissions.
- user id 1000 - 65535

  
#### Add a new user
````
adduser steve
````
or 
````
useradd -m <username>
````
#### Set or change a user password
````
passwd <username>
````

#### List All Users
````
cat /etc/passwd
```` 
#### Important Files for Users

**/etc/passwd**
- Stores user account information

![image](https://github.com/user-attachments/assets/8573faaf-b158-4699-9abd-48b9ae43c2d8)



#### Modify an Existing User

**Assign a Customized UID to a User**
````
usermod -u 3000 tony
````

**Change user login shell**
````
usermod -s /sbin/nologin steve
````
**Add a Comment**
````
usermod -c "development team" bruce
````
**Lock a User's Password** (Prevents the user from logging in.)
````
usermod -L natasha
````
**Unlock a User's Password**
````
usermod -U natasha
````

