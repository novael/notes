Setting up local Git server
---------------------------
http://blog.goosoftware.co.uk/2012/02/07/quick-git-server/

Alias commands
--------------
git config --global alias.<alias> command

Set up a remote repo and do initial push
----------------------------------------
**On remote server**  
`ssh git@<server>`  
`mkdir <project>.git`
`cd <project>.git`
`git init --bare`

**On local machine**   
`cd <project>`   
`git init`  
`git add .`  
`git commit -a -m "Commit message"`  
`git remote add origin git@<server>:<project>.git`  
`git push origin master`
