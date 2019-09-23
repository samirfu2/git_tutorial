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
  3. >> git clone "url_repository_name" (It will copy the directory form git repo- not need to do git init and git remote add origin "<URL         to repository>")
  4. >> git pull origin master (This will pull the file from origin to local repository-- use full when multiple developer wil working for         same project, one of the developer wanted to update there local repos before starting new development)
### Git Branches
  
