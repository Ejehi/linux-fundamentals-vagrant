# linux-fundamentals-vagrant

## Seting Up a Vagrant Server
![alt text](https://github.com/Ejehi/linux-fundamentals-vagrant/blob/main/Seting_Up_a_Vagrant_Server.png "Seting Up a Vagrant Server")

This screenshot shows the process of initializing a Vagrant environment with Ubuntu (vagrant init hashicorp-education/ubuntu-24-04 --box-version 0.1.0), starting the virtual machine (vagrant up), and connecting to it via SSH (vagrant ssh). This sets up a portable and reproducible development server for Linux-based tasks.

## Exploring the Linux File System

![alt text](https://github.com/Ejehi/linux-fundamentals-vagrant/blob/main/Exploring_the_Linux_File_System.png "Exploring the Linux File System")

This screenshot shows the creation of a custom folder structure inside the Vagrant VM. I created a **projects** directory inside the vagrant user's home, with a nested **devops** folder. 

## Managing File Permissions and Ownership

![alt text](https://github.com/Ejehi/linux-fundamentals-vagrant/blob/main/Manage_File_Permissions_and_Ownership.png "Managing File Permissions and Ownership")

This screenshot shows how file permissions and ownership are managed in Linux. The file **linux_fundamentals.txt** was given permission 600 using chmod, meaning only the owner can read and write to it. The file **linux_fundamentals_2.txt** was given permission 644 using chmod, meaning the owner can read and write to it, and the group and all other users can only read the file. The chown command changed both files' owner to root. The ls -l output confirms the changes: 
- The first field for **linux_fundamentals.txt** (-rw-------) indicates permissions, and root root shows the user and group ownership.
- The first field for **linux_fundamentals_2.txt** (-rw-r--r--) indicates permissions, and root root shows the user and group ownership.

## Installing and Configuring a Package
Installing a basic package with apt

![alt text](https://github.com/Ejehi/linux-fundamentals-vagrant/blob/main/Install_and_Configure_a_Package.png "Installing and Configuring a Package")

## Testing Remote Connectivity

![alt text](https://github.com/Ejehi/linux-fundamentals-vagrant/blob/main/Test_Remote_Connectivity.png "Testing Remote Connectivity")

This screenshot shows the result of using the ping command to test connectivity to google.com from inside the virtual machine. The output confirms that the remote server is reachable, with 0% packet loss and an average round-trip time of ~193 ms. This is useful for diagnosing network connectivity, ensuring DNS is working, and measuring latency to external servers.
