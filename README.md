# GitHub Tutorial

_by Michael Gierlach_

---
## Git vs. GitHub
  Git is the basic workflow that runs in the command line. It keeps a snapshot of your code. 
You do not need Github in order to use Git. When we initize git, we can edit files, add them and commit them.
  Github is a website stores your code and tracks all your changes. It also collaborates with other files. You need git in order to use Github. 






## Initial Setup
#### In order to make a Github account,
1. Click sign up 
2. Make a username (the same as your HSTAT username)
3. Make a password (the same as your HSTAT password)
4. If theres a bubble saying something went wrong, **ignore it and keep going**
5. Make a _free_ account
6. Then press finish the sign up
7. Then, you go to c9.io
8. click the gear icon
9. Press connected services
10. Connect to your Github  

#### In order to make an SSH key
1. On the top right corner on Github, click on your profile icon and then on settings
2. On the left sidebar, click SSH and GPG keys
3. New SSH key
4. Make the title cloud9
5. On KEY, witch to the cloud9 tab, on the top right, press the gear icon
6. Click on the SSH key tab and copy and paste your SSH key into Github 
7. Add the SSH key 
8. On cloud9, open github-learning IDE
9. ssh -T git@github.com
10. It is going to give you a message that you authenticated but Gitbug does not provide shell access  

---
## Repository Setup
#### In order to make your first repo
1. `Make cd ~/ workspace` which will take you into a directory
2. `Mkdir my-repo`; this will make a directory where you can put in things like files
3. `Cd my-repo`; this will put you inside the directory and it will allow you to make files
4. `Git init`; This will initialize the directory turning it into a repository which is the local repository. 
   You are then able to push it to a remote repository to save and so others can see what you commited and done on Github.  

#### In order to add files into the repository
1. Touch my-file.txt which will make a text file called "my-file".
2. Open the file and type whatever you want
3. Make sure the file is saved
4. Git add my-file.txt which will add the file to the staging area. This is where we can add and make changes to the files
5. Make sure to type git status to see if your text in the file is ready to be commited.
6. git commit -m "make a file" will take whatever is in the staging area and it will add to the remote repository on Github. The message should be short and simple, it should get straight to the point.  

#### In order to make a remote repository
1. Go to Github
2. Click on the "+"
3. Click on new repository
4. Type in your local repository name. **THE NAMES SHOULD ALWAYS MATCH**.
5. Press create repository
6. If you are asked to vertify your email then do it, if not don't worry about it
7. Click SSH on the top and copy and paste each line of code one at a time
8. Lastly, go back to Github and open the repository and you should see the changes on your website.


---
## Workflow & Commands
* `_Git status_`: It is an optional command that shows which files have been edited since the last commit (They will be red) `git status`
* `_Git add_`: Adds files to the stage so it can be commited `git add`
   *` _Git add._` : Adds the current or entire file(s) to the stage `git add.`
   * `_Git add --all_` : Includes all changes including deleted files `git add --all`
* `_Git push_`: Sends the local repository commits to the remote repository or up to the cloud `git push