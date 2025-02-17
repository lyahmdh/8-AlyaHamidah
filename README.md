# BCC-Git-Github-DS
<p align="center">
  <img width="100%" src="pic/img_git.png" alt="pic1">
</p>
Hello fellow BCC interns and aspiring developers! 

This BCC Git & GitHub Tutorial repository is your friendly guide to mastering version control with Git and collaborating efficiently using GitHub. Here, you'll learn fundamental concepts such as repositories, branches, commits, merges, pull requests, and more to build a solid foundation for managing code collaboratively.

## What You'll Learn
By following this step, you will learn:

- **Creating a Repository:**
  - How to set up a new repository on GitHub.
- **Cloning an Existing Repository:**
  - How to copy a GitHub repository to your local system.
- **Making Changes and Pushing to GitHub:**
  - How to create, track, and upload changes to your repository.
- **Branch Management:**
  - How to create, switch, and list branches for better collaboration.

## Windows Installation

1. Download Git
- Visit the official Git website: [Git](https://git-scm.com/downloads) for Windows 
- Click the download button to get the latest installer.

2. Install Git

- Open the downloaded .exe file.
- Follow the installation wizard, keeping the default settings unless you need custom configurations.
- Ensure that "Git Bash" and "Git GUI" options are selected during installation.

3. Check Version
- Open Git Bash or Command Prompt and run:
```bash
git --version
```
(just move or try linux hehehehe)

## Linux Installation

1. Before using Git, you need to install it on your system. Open terminal and Follow the steps below to install Git on a Debian-based system (e.g., Ubuntu):
```bash
sudo apt get-update  # Update package lists  
sudo apt install git  # Install Git
```
2. Check Version
```bash
git --version
```
## Basic Git Setup
Whether you use Windows or Linux the only difference is in the installation process. Once Git is installed, all the commands and steps remain the same across both operating systems.
1. Set Up Your Name and Email
```bash
git config --global user.name "Your Name" #Fill with your name (U can use your username github)
git config --global user.email "your.email@example.com" #Fill with your gmail
git config --global --list #Check your list
```
2. Initialize a Git Repository
```bash
mkdir test-ds-git #make a file
cd test-ds-git  
git init 
git status #Check if you successfully initialized a Git repository
```
Possible Output:

  On branch master

  No commits yet

  nothing to commit (create/copy files and use "git add" to track)

3. Create and Commit a File
```bash
echo "World Hello" > hello.txt  # Create a new file named hello.txt  
git add hello.txt  # Stage the file to be included in the next commit  
git commit -m "First commit"  # Save the changes with a meaningful commit message
```
Possible Output:

[master (root-commit) 213883c] First commit

 1 file changed, 1 insertion(+)
 
 create mode 100644 hello.txt


## Basic Github
1. Create Repository
   - Go to GitHub and log in.
   - Click New Repository -> Enter a repository name -> Choose Public or Private -> Click Create repository.
<p align="center">
  <img width="100%" src="pic/S1.png" alt="pic2">
</p>

You can choose between 

2. Clone an Existing Repository
```bash
cd
mkdir ds-github
cd ds-github
git clone https://github.com/your-username/your-repo-name.git  
cd your-repo-name
```
2. Use the Token for Git Authentication
```bash
git remote set-url origin https://YOUR_GITHUB_USERNAME:TOKEN@github.com/YOUR_GITHUB_USERNAME/YOUR_REPO.git
git fetch
```
How to get the token ? <br>
i. First go to the profile and go to setting
<p align="center">
  <img width="100%" src="pic/S2.png" alt="pic3">
</p>
ii. After that scroll down and search for 'developer settings'
<p align="center">
  <img width="100%" src="pic/S3.png" alt="pic4">
</p>
iii. From there click Personal Access Tokens and go to generate new token , choose "generate new token classic"
<p align="center">
  <img width="100%" src="pic/S4.png" alt="pic5">
</p>
iv. Name the token whatever u want and check some permission that you need and click generate token
<p align="center">
  <img width="100%" src="pic/S5.png" alt="pic6">
</p>

3. Make Changes and Push to GitHub
```bash
touch test.py
git add .  # Stage all changes  or u can use git add test.py
git status # You can see the changes
git commit -m "Add file test.py"
git push origin main
```
4. Create a New Branch
```bash
git branch #Check current branch
git branch -a #List all branches	
git checkout -b new_branch #Create & switch to a new branch	
git switch main # Switch to an existing branch	
```
5. Push and Delete a Branch
```bash
git push origin new_branch #Push new branch to github repo
git branch -d new_branch #Delete a local branch	
git push origin --delete new-feature #Delete a remote branch
```
6. Pulling the Newest Changes
```bash
git fetch  # Retrieve the latest changes from the remote repository without merging them
git pull origin main  # Fetch and merge the latest changes made by your collaborators
git pull origin <branch-name>
```

## Video
-Still confused? You can watch a 40 minutes GitHub tutorial for a clearer understanding. [Full Youtube Video](https://www.youtube.com/watch?v=tRZGeaHPoaw&t=725s)


## Bonus
- git merge -> Combine changes from one branch into another. (Be careful with conflicts! You need to resolve them first before you can successfully complete the merge.)
- git log -> View commit history.
- git reset <file> -> Unstage a file before committing.
- git stash -> Temporarily save uncommitted changes.


### Note:
I highly recommend starting with the basics and using the CLI version of Git. Once you're familiar with it, you can transition to [GitHub Desktop](https://desktop.github.com/download/) for a more visual experience. (still i love CLI)

## Assignment
1. Make your own repository for personal use and you can use that repository to clone another material in the future. <br> You can use this format : TeamNumber-YourName (Use Full Name)
   ex = 1-Pieter  
3. Set up a team repository to collaborate and store code with your team. <br> You can use a structured format like this: TeamNumber-MemberName1-MemberName2 (Use FullName)
   ex = 1-Pieter-Toni

## Source:
- [Git](https://git-scm.com/docs/gittutorial)
- [Git](https://docs.github.com/en/get-started/getting-started-with-git/set-up-git)
- [Github](https://docs.github.com/en/get-started)










