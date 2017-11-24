# mysql-server-setup
  Usage:
 ```bash
#Give perms to the current user to execute script
chmod u+x ./mysql-server-setup

#Run the script (must have account password)
./mysql-server-setup
```  
  Original tutorial: https://www.linode.com/docs/databases/mysql/install-mysql-on-ubuntu-14-04  
  Tested on Ubuntu 16.04  
  Raw code: 
```bash
#!/bin/bash  
sudo apt-get update  
sudo apt-get upgrade  
sudo apt-get install mysql-server  
sudo mysql_secure_installation  
mysql -u root -p  
sudo service mysql stop  
sudo dpkg-reconfigure mysql-server  
sudo service mysql start  
sudo apt-get install mysqltuner  
mysqltuner  
``` 
