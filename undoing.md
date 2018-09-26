# :man_facepalming: Undoing

:point_left:[BACK](../README.md)

### Amend the message of my last commit

Git Commnad 	        		  		    | Description
------------------------------------------- | ---------------
**`git commit --ament`** 			  		| follow prompts to change the commit message, save and exit using `:x`

### Accidentally committed to the wrong branch

Git Commnad 	        		  		    | Description
------------------------------------------- | ---------------
**`git reset HEAD~ --soft`** 			  	| undo the last commit, but leave the changes available
**`git stash`** 						  	| stash changes
**`git checkout correct-branch`** 	  	    | move to the correct branch
**`git stash pop`** 					  	| apply stash
**`git add . # or add individual files`**   | add changes to correct branch
**`git commit -m "your message here"`** 	| now your changes are on the correct branch

### Accidentally committed to the wrong branch (Cherry-Pick)

Git Commnad 	                        	| Description
------------------------------------------- | ---------------
**`git checkout correct-branch`**        	| move to the correct branch
**`git cherry-pick master`**		        | grab the last commit to master
**`git checkout master`**	  				| move to master
**`git reset HEAD~ --hard`**				| delete it from master

[:point_left:BACK](../README.md)