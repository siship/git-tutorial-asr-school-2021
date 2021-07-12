# Git tutorial | [IEEE SPS Summer School 2021](https://sites.google.com/iitdh.ac.in/vssasr2021) on ASR

## What is git?

Git is a distributed version control system. It facilates merging of different source codes from different developers. And codes are distributed among developers. Make a copy of the repository in your local machine and work offline, and then push your changes to the server. 

- Distributed version control system
- Trunk based development
  - Working in different versions simultaneously


Install Git in your PC
- Linux
```shell
sudo apt-get update
sudo apt-get install git
git --version (for checking Git version)
```
- Windows
  - Download Git installer from following link and install
  - https://gitforwindows.org/

Set-up Git in your PC
```shell
git config --global user.name "username" 
git config --global user.email "youremail@domain.com" 
git config --list
	user.name=username
	user.email=youremail@domain.com
```
You can see all the configuration done for your git account from the .gitconfig from you Home directory
```shell
gedit .gitconfig
```

Clone a repository
```git clone https://github.com/jagabandhumishra/IEEE-Summer-School.git```

To specify a directory, where you want clone the repository (e.g., I want download in ```/home/sishir/ASRREPO```)
```git clone https://github.com/jagabandhumishra/IEEE-Summer-School.git /home/sishir/ASRREPO```

- Create GitHub Repository
- Creat a file
  - commit changes
- Create branch
- Merge the branch with master
  - Go to the repo and click ```Compare & Pull Request```
- What if other person wants to contribute with your project
  - Fork and create pull request

- This command lists all the files that have to be committed.
  - ```git status```
- This command lists all the local branches in the current repository.
  - ```git branch``` 
- This command creates a new branch.
  - ```git branch [branch name]  ```
- The git add command adds a change in the working directory
  - ```git add (file names)``` Or ```git add .```
- This command records or snapshots the file permanently in the version history
  - ```git commit -m "(committed message)"```
- This command sends the committed changes of master branch to your remote repository.
  - ```git push -u origin master ```
- This command shows the differences between the two branches mentioned
  - ```git diff [first branch] [second branch]```

- This command fetches and merges changes on the remote server to your working directory.
  - ```git pull [Repository Link] ```

For creating a new branch
```shell
git checkout -b testbranch
git add .
git commit -m "test"
git push origin testbranch
```
For merging with main/master branch
```shell
git checkout main
git merge testbranch
git push
```
