# :alien: Not git 

:point_left:[BACK](README.md)

### 1.Usefull macOS terminal commands 

Command     	        		  			| Description
----------------------------------------- 	| ---------------
**`sudo lsof -i :<port>`** 			  		| list processes running on specific port
**`lsof -i -n -P \| grep TCP`** 			| list TCP ports in use
**`sudo pkill mysql`** 			  			| Kill mysql
**`sudo nano /etc/hosts`** 			  		| manage local hosts


### 2. MYSQL commands

Commnad 	 	        		  																																	   | Description
---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------
**`mysqldump --single-transaction -q -h <ip_address> -u <user> -p --default-character-set=utf8 --skip-triggers --set-gtid-purged=OFF --no-create-db <db>`** 		   | dump database
**`mysqldump --single-transaction -q -h <ip_address> -u <user> -p --default-character-set=utf8 --skip-triggers --set-gtid-purged=OFF --no-create-db <db> > <db_new>`** | dump database to file 

### 3. Reseting MYSQL 'root' user password 

Commnad 	 	        		  																																	   | Description
---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------
**`mysqld stop`** 		   | stop mysl server
**`sudo /usr/local/mysql/bin/mysqld_safe --skip-grant-tables`** |  Start the server in safe mode with privilege bypass
**`sudo /usr/local/mysql/bin/mysql -u root`** |  In a new terminal
**`update user set authentication_string=PASSWORD("<new_password>") where User='root';`** |  Update the root user pasword
**`flush privileges;`** |  Flush privileges
**`\q`** |  Quite mysql
**`mysqld restart`** |  Restart mysql server
**`mysqld -u root -p<new_password>`** |  Restart mysql server
**`set password=password('<new_password>')`** |  Set new password when asked: You must reset your password using ALTER USER statement before executing this statement.



:point_left:[BACK](README.md)