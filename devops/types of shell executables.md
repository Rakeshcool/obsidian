- sh
- bash(preferred)
- ksh(obsolete)
- dash(relatively new is being used for some os like latest version of ubuntu)


#!/bin/bash or #!/bin/sh are linked 


## [[#!/bin/bash]] shall be used in the script at first

## permission:

|Value|Permission|
|---|---|
|4|Read Permission|
|2|Write Permission|
|1|Execute Permission|

### 3)What are the different types of permissions in Linux, and what do they mean?

There are three types of permissions in Linux: 

read **(`r`)**

write **(`w`)**

execute **(`x`)**

They are applied to:

owner **(`u`)**

group **(`g`)**

other **(`o`)**

### **4) What is “chmod 777 “, “chmod 755” and “chmod +x “or “chmod a+x”?**

**Chmod 777 [file_name]**

This command gives all three permissions to everyone (owner, group and other)

**chmod a+x [file_name]**

It makes a file executable for everyone. It is the most used command after we install an executable file, we still need to add a permission to actually make it an executable file.

**chmod 755 [file_name]**

### 5) How can we revert changes made by “chmod” command in Linux?

To undo or revert changes made by “chmod” command in Linux , we can use the **`chmod`** command again but this time we should mention the correct permission we want. 

 Here are the steps to undo or revert changes:

- Determine the correct permission you want and use `chmod` command again.   
    For Example: If we want to revert the changes to “rw-r–r–” (read and write permission for owner, read-only permission for group and others), according to this our octal value would be “644” (read = 4, write=2).
- Now open the directory and write the given command :

**chmod 644 [file_or_directory_name]**