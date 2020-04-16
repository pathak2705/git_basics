git add -> a cache of files that you want to commit - helps to manage between what to commit and what to not
eg- git add xyz.html

git commit  -> takes a snapshot of our file ready to be pushed
eg- git commit -m "message"

git push -> pushes the file from local to remote repository

git pull -> pulls file from remote to local repository

git status -> shows the difference between local and and remote files

git log -> gives a log data of all commits

git revert HEAD -> takes the file back to just previous version/commit
	(*note that redoing it will take file to the latest version again)
	
*merge conflict -> to promote collaborative workspace, git provides a feature known as merge conflict
                   When we commit something locally without pulling the latest remote version of the file
				   then Git places this as a merge conflict and merges our file with both versions where
				   text between <<< and === is local change and text between === and >>> is remote change.
				   Hence, we can see both versions simultaneously and accept/reject a version according to 
				   our requirements.
				   (*note first pull then do any commits)
                   				   