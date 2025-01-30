## Task : File Permissions

-  Create a group named **hogwarts**
-  Create users: **harry, hermione, ron and luna**
-  Add user harry, hermione and ron to the hogwarts group.

-  Create a directory named **documents** in the root (/) directory.
-  Assign ownership of the documents directory to the harry user and the    
    hogwarts group.

-  Set the permissions of the documents directory to **rwxr-x---** using chmod.
-  Ensure that only the owner (harry) can read, write, and execute within the    
   documents directory, while members of the hogwarts group can only read 
   and traverse (cd) into the directory.

-  Configure a umask value that ensures new files created within the 
   documents directory have permissions **rw-r-----**

-  Set an ACL on the documents directory to grant **luna** user the ability to  
    modify (write) files within the directory, even though they are not the 
    owner.

-  As the harry user, create a **sample.txt** document within the documents 
     directory.
-  Verify that the **luna** user can modify the file 
     Confirm that the **hermione** user cannot modify the file.
