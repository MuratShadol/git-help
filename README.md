# Repository for GitHub functions and useful commands

## First steps 

Install git, if you are on Windows. Now you have command line.  
Open terminal (command line).  

---

### Commands for command line

Navigate to directory:  
``` Bash
cd path/to/your/folder
```

Navigate to home directory  
```Bash
cd ~
```

Create file:  
```Bash
 touch file.*
```

Open file for editing. If file doesn't exist it creates and opens new file:  
```Bash
nano %your-file%
```

Create folder:  
```Bash
mkdir %folder-name%
```

Remove file:  
```Bash
rm %file-name%
```

Remove empty folder:  
```Bash
rmdir %folder-name% 
```

Remove folder with files:  
```Bash
rm -R %folder-name%
```

List content of current folder:  
```Bash
ls
```

List all content in folder (including hidden files/folders):  
```Bash
ls -a 
```

Copy/Move file:  
```Bash
cp %what-to-copy% %what-to-copy% ... %where-to-copy%  
mv %what-to-move% ... %where-to-move%
```
---

## Create repository in GitHub

Go to [GitHub](https://github.com "I am GitHub!") Sign up or sign in, if you have an account.  
Navigate to your profile-repositories-New, choose the name of your repository, make it public or  
private.

---

## Git 

Now you need to install Git.  
For Linux users in command line type  
```Bash
sudo apt-get install git  
sudo add-apt-repository ppa:git-core/ppa  
``` 

Now all you need to do is to navigate to some folder, then type *git init*. This command 
makes current folder as git-depended. Now create SSH key in your GitHub. This key is needed for 
synchronization between local repository and remote repository. Ones you connect them 
you can create files, edit them and load to remote repository on GitHub.

---

## Git commands 

Ones you created files using standard command line functions *touch/nano*. You can upload them to
GitHub repository. To do that follow these steps:  

* ``` git status```. This command will give you information about current status of repository.  
* ``` git add %file-name%```. This command prepares files to be uploaded on GitHub.  
* ``` git commit -m %comment%```. This command saves updates in file.  
* ``` git push```. This command uploads files to GitHub.  

Ones you done that you should be able to see your files on GitHub repository. 

---

# File status/Commit navigation

```bash git log``` This command will list information about all commits in the project.

You can see the sequence of letters and numbers. This is a hash. Hash is a fingerprint of commit  
It contains information about commit: when it was done, files content in the repo at the time  
of the commit, link on parent commit. Hash is the main id of the commit.

Also ```bash git log``` displays the author, the date and the message of the commit. To get compact  
version type ```bash git log --oneline```. It will print the same information in more compact way.  

HEAD is a file in .git directory, this file contains link to the hash of the last commit. You can use  
HEAD instead of last commit' hash. 

## Statuses

```bash git status``` Will display information about files. This information contains file status.


```mermaid
graph LR;

untracked -- "git add <file>" --> staged;
staged -- "git commit -m "message" --> tracked/commited;
staged -- "Changes in file" --> modified;
modified -- "git add <file>" --> staged;
tracked/commited -- "Changes in file" --> modified;

```

This is the lifecycle of GitHub file.








































