# :steam_locomotive: git-cheat-sheet :steam_locomotive:
Useful git commands!

## Accidentally committed to the wrong branch

Git Commnad 	        		  	| Description
----------------------------------- | ---------------
git reset HEAD~ --soft 			  	| undo the last commit, but leave the changes available
git stash 						  	| stash changes
git checkout correct-branch 	  	| move to the correct branch
git stash pop 					  	| apply stash
git add . # or add individual files | add changes to correct branch
git commit -m "your message here" 	| now your changes are on the correct branch

## OR with Cherry-Pick

Git Commnad 	                    | Description
----------------------------------- | ---------------
git checkout correct-branch         | move to the correct branch
git cherry-pick master		        | grab the last commit to master
git checkout master 	  			| move to master
git reset HEAD~ --hard				| delete it from master

## Discarding local changes (permanently)

Git Commnad 	            		| Description
----------------------------------- | ---------------
git checkout -- `file` 				| discards local changes in a file (permantently)
git checkout -- .      				| discards local changes in all file (permantently)	


