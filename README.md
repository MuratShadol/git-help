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

* ```Bash git status```. This command will give you information about current status of repository.  
* ```Bash git add %file-name%```. This command prepares files to be uploaded on GitHub.  
* ```Bash git commit -m %comment%```. This command saves updates in file.  
* ```Bash git push```. This command uploads files to GitHub.  

Ones you done that you should be able to see your files on GitHub repository. 

---

Good luck in exploring GitHub features! 
