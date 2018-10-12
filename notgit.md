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


:point_left:[BACK](README.md)