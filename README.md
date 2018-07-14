# DS_Challenge


## Git tutorial

### Clone and fork repository  
1. Fork or create repository on github website
2. Open Terminal/command prompt.  
3. Navigate to the location you want to put the folder
``` $ cd folder_location ```  
4. Download the github repository to local folder  
``` $ git clone GitHub_repository_link```  
5. Change directory to local folder
``` $ cd GitHub_repository_link ```
   
<<<<<<< HEAD
4. Make changes
*. git pull


5. Git add .
6. Git commit -m “comments”
7. Git push
=======
### Stores the current contents  
1. Make changes in local folder
2. Stage the file for commit to your local repository.
``` 
$ git add .  # add all files to git version control
$ git add -u  # add updated files to git version control
```  
3. exclude folder contains data  
``` $ git reset -- Data_folder/  ```   
4. Commit the file that you've staged in your local repository. Commits the tracked changes and prepares them to be pushed to a remote repository. 
``` $ git commit -m "Add existing file" ```  
5. Push the changes in your local repository to GitHub.  
``` $ git push ```  


### Resolve a conflict
1. Undo the merge and pull again.
	To undo a merge:  
	``` 
	$ git merge --abort [Since git version 1.7.4]  
	$ git reset --merge [prior git versions]  
	 ```
2. Resolve the conflict.
3. Don't forget to add and commit the merge.
4. git pull now should work fine.


### Keep your fork synced    
When collaborate with teammates, in order to propose changes to the upstream, or original, repository. In this case, it's good practice to regularly sync your fork with the upstream repository.  

#####Step 1: [Configured remote repository for your fork](https://help.github.com/articles/fork-a-repo/) (one time)  
##### Step 2: [Syncing a fork](https://help.github.com/articles/syncing-a-fork/)  
1. Open Terminal/command prompt.
2. Change the current working directory to your local project.  
``` $ cd GitHub_repository_link ```  
3. Fetch the branches and their respective commits from the upstream repository. Commits to master will be stored in a local branch, upstream/master.  
``` $ git fetch upstream  ```  
4. Check out your fork's local master branch.  
``` $ git checkout master ```  
5. Commit your local changes  
``` $ git commit -m "some comments" ```  
6. Merge the changes from upstream/master into your local master branch. This brings your fork's master branch into sync with the upstream repository, without losing your local changes  
``` $ git merge upstream/master ```

>>>>>>> upstream/master
