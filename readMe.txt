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
		   
git commit -am file_name"message" -> adds and commits simultaneously
eg- git commit -am readMe.txt"message"

git branch -> lists out all the branches made in a project

git branch branch_name -> adds a new branch to current project
eg- git branch feature

git checkout branch_name -> moves the HEAD pointer(current pointer) towards the named branch
eg- git checkout master

git checkout commit_hash -> takes the HEAD pointer to the given commit
                            You can either start working on this by making a new branch or switch to another branch to discard it.
			    
git switch - -> this will undo the just previous command written 

git merge branch_name -> merges the given branch with current branch

git push --set-upstream origin branch_name -> when there are more than one branch in a project, user has to specify which
                                              branch to push
                   				   
