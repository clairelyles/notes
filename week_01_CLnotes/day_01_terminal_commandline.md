##Day 1 Notes
###11/17/14

### Terminal & Command Line

**What is Terminal?**

* text editor & interface with computer

**What is HomeBrew?**

* a package manager
* allows you to dynamically install packets
* access to command line utlities
* installs rails, utlities for rails, etc

**Command Line**

all command lines are mini programs

* ```ls``` lists the folders
* ```ls -a``` listing of files & hidden files
* ```ls -al``` files, hidden files & date stamp
* ```.zshrc``` updates to terminal will
* ```pwd``` tells you the dir you're in
* ```cd ~``` or ```cd``` takes you back to the home folder
* ```touch file_name``` to create a new file
* ```suvl``` shortcut for openeing sublime!!!
* ```cp``` copy 
	* **orig_file_name** **new_file_name**
* ```mv``` move 
	* ```mv file_name taco``` moves file to taco folder within root
	* ```mv file_name ./taco``` moves file to taco folder within root
	* ```mv file_name file_name2``` rewrites file_name to file_name2
* ```rm``` removes file
	* ```rm - rf``` removes a whole **folder**
		* ```r``` is recursive and ```f``` force removes the files without prompting for confirmation
* ```./open``` opens a file
* ```cat``` reads a file within terminal
* ```grep``` history | grep git basically looks through your history and retrieves every command line that contains "git"
* ```piping | ``` fortune | cowsay takes the output from fortune and pipes it into cowsay!
* ```ctrl + l``` clears terminal
* ```head``` returns the first 10 lines of the file.
	+ ```-n``` indicates the # of lines desired to be read (e.g. ```head -n15 file_name``` or ```head -n 15 file_name``` returns the first 15 lines
		
***
Don't forget dusk notes on Git Repo
***

###Git

[img][http://greenido.files.wordpress.com/2013/07/git-local-remote.png?w=696&h=570]

**What is it?**

It's a form of version control. Projects exist on Github and manage the "forks" or revisions for easy merging, editing, etc...

**Git vs Github**

* Git = a tool and set of command line utlilties that allow you to navigate between files. Save, update and revert back to code.
* Github = hosting/social media. Sharing and caring between developers.

**Git**

* Cloning
	* Clone a document into you're home directory by ctrl + c the SSH clone URL from Git and ctrl + v using ```git clone git@github.com:wdi-sea-01/URL.git```. Bassically you're virtually grabbing documents from Git and pulling them onto your MacBook.
* Fork
	* To fork a project (take the source from someone's repository at certain point in time, and apply your own diverging changes to it. Only exists on GitHub.
* Pull
	* fetches new data from Git as the file you cloned becomes updated
* Commit
	* Will not show up in Git until home files are "committed"

**Create a new Git Folder**

Use ```git init``` to create a new folder on the remote Git server. ```git status``` checks to see if files have been pushed. "Untracked" files have not been pushed onto the Git server.

**Git Status**

Git *add* will add files to the Directory. Git *commit* adds them to the Git repository!


```git add -A``` adds all the files within the folder to be tracked and committed.

```git commit -m file_name "Insert string here..."``` adds a hard comment to the specified file_name that you modified
OR

```git commit -am "Insert string here..."``` (if no new files have been edited/deleted) adds a hard comment to ALL the modified files

###Pushing

Pushing pushes files from your computer onto Git. 

* Add new repository on Github
* Initalize README
* Add .gitignore Node

```git remote -v``` will show all repositories that are fetched or pushed from Git

1. Create new repo on Github
2. Go to README and copy node
3. In terminal, go to folder you want to push to Git. Once in folder, initialize git using ```git init```
4. Git will be connected to folder
5. Run ```git status``` to check if any files are untracked
6. To track files run ```git add -A```
7. Run ```git status``` to check if files are tracked
8. Commit files using ```git commit index.html -ma "Edited index"```
9. input Git remote add origin
10. Run ```git remote -v``` to see where files were pushed and pulled from

*Note when you clone a repository you no longer need to  recconect to git, simply just push up to git using ```git push```




