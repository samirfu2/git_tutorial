# git_tutorial

# What is git
  Git is a distributed version-control system for tracking changes in source code during software development. 
### How to start with GIT
1. create dev_dir in your local system
2. Run Command:  
  >>  git init  (Once you will do this , this directory will be tracked by GIT)
3. To test : you can create any file under your created directory
4. >> git status (To check how many files from the local directory it is tracked by git -- Untracked means not added to stage )
5. >> git add [file_name] (Now given file name is added to stage, it is before the commit)
    Note: The git add command move to file from  DEV---> STAGE
6. >> git commit -m "Message for commit"  (This will take the file from stage and moved this to the local repository , after this command       now we will not see anything from git status command)

7. Now everything is ready in our local , we can start pushing our changes to remote repository, for that we need repository link/path
   if the repository path is not available than you can create new repository after signing the git web.
   
8. >> git remote add origin "<URL to repository>" (this will add the git repository path , where you will be pushing the code)
     example:  git remote add origin "http://github.com/...../repos_name.git"
9. How to push the file to repository
   >> git push origin master
10.  If at all you change any commited file just you need to apply
   >> git commit -m "update-message"  (This will push to local repository not to git location)
   >> git push origin master (To push to git repository)
### How to clone the repository 
    Suppose you wanted to take some once code to you dev folder, for that you need to clone the repository
  1. Create your local directory using mkdir "folder_name"
  2. change to folder_name (cd folder_name)
  3. >> git clone "url_repository_name" (It will copy the directory form git repo- not need to do git init and git remote add origin "          <URL to repository>")
  4. >> git pull origin master (This will pull the file from origin to local repository-- use full when multiple developer wil working for         same project, one of the developer wanted to update there local repos before starting new development)
### Git Branches
    This is use full when multiple developer is working 
 1. >> git branch <name_of_the_new_branch> (Create and use: Any developer can work on branch and after that they can merge the brach to    
     master - The last commit to the master will be the first commit to the git branch)
 2. >> git brach (List all the branches)
 3. >> git branch -D <branch_name> (Simply to delete the branch)
 4. >> git checkout branch_name (To switch to the new brach from current branch)
 5. >> git push origin branch_name (Pushed the new file to branch_name)
### Git Log 
     To check the history of the git 
  1. >> git log (It will display the logs of the brach or master depends on where you are currently)
  
### Git Stash
     Do not want to save your work space to your git repository. To Stash you staged  files without committing just type 
  1. >> git stash ( It is remove all the current changed files which is under local repository and also to stash the untracked file as           well )
  2. >> git stash pop (If you wanted to get back the old changes , it is like undo of git stash)
### Git Revert
   1.  git log (It will display the commited logs and with ID)
   2.  git revert <commited ID from above> (It will reverted to the commited ID) 
   3.  git checkout <commited ID from above> (To check what changes)
### Git Diff
    
