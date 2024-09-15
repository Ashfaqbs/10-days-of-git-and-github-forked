
</div>

## Basic Command Lines

Developers need to know basic Unix commands. Some tasks necessary need to be done using git bash, mac terminal, or window command prompt. In this tutorial, we will use git bash to learn the basics of the Unix command which you may need as a developer. This is not an exhaustive list but it is enough for daily uses. To make use of git bash first you should install [git](https://git-scm.com/). You can install by just clicking the next button up to the end of the installation.

If you prefer watching the tutorial, click this [link](https://www.youtube.com/watch?v=9cCApTLb_Io&list=PLbvhRHYrmshSCAHZbibqh_px_LxnU54dk)

### Current working directory

Checking the working directory using the command _pwd_.

```sh
 MINGW64 ~$ pwd
/c/Users/Ashfaqbs
```

### Navigating directory

Now, let's go to the Desktop using cd(change directory).

```sh
 MINGW64 ~$ cd Desktop
 MINGW64 ~/Desktop
```

To check where you are at, use the _pwd_ command age

```sh
 MINGW64 ~/Desktop$ pwd
/c/Users/Ashfaqbs/Desktop
```

We use _cd_ to get into a directory(folder) and we use _cd.._ to get out from a directory, in other words, we use _cd_ to go forward into a directory and _cd .._ to go backward from a directory.

### Making Directory

Now, let's create a directory inside the Desktop. Call the name of the directory, 10-days-of-code. You give it any name but I am in favor of this name.
Use the _mkdir_ command to make a directory(folder)

```sh
 MINGW64 ~/Desktop$ mkdir 10-days-of-code
```

Now let's go to the 10-days-of-code folder using _cd_ command.

```sh
 MINGW64 ~/Desktop$ cd 10-days-of-code
 MINGW64 ~/Desktop/10-days-of-code
 MINGW64 ~/Desktop/10-days-of-code$ pwd
/c/Users/Ashfaqbs/Desktop/10-days-of-code
```

### List files and directories

We can check the files and directories we have in a directory(folder) using the _ls_ command.

```sh
 MINGW64 ~/Desktop/10-days-of-code$ ls
```

No files or directories were found in the 10-days-of-code folder because we didn't create them yet. Let's create some directories

```sh
 MINGW64 ~/Desktop/10-days-of-code$ mkdir day-1
```

Now let's check if there are some files or directories in the 10-days-of-code folder.

```sh
 MINGW64 ~/Desktop/10-days-of-code$ ls
day-1
```

Now, you see a day-1 folder that you created.

Now let's create multiple folders at one and use _ls_ to see all the directories we have in the 10-days-of-code folder.

Making multiple folders at once

```sh
 MINGW64 ~/Desktop/10-days-of-code$ mkdir day-2 day-3 day-4 day-5 day-6 day-7 day-8 day-9 day-10
```

Using _ls_ we can see all the directories we have in the 10-days-of-code

```sh
 MINGW64 ~/Desktop/10-days-of-code
$ ls
day-1  day-10  day-2  day-3  day-4  day-5  day-6  day-7  day-8  day-9
```

### Detail list

Let's see a detailed list of the directories using multiple commands, _ls -la_.

```sh
 MINGW64 ~/Desktop/10-days-of-code
$ ls -la
total 20
drwxr-xr-x 1 Ashfaqbs 197121 0 Jan 19 02:16 .
drwxr-xr-x 1 Ashfaqbs 197121 0 Jan 19 02:05 ..
drwxr-xr-x 1 Ashfaqbs 197121 0 Jan 19 02:12 day-1
drwxr-xr-x 1 Ashfaqbs 197121 0 Jan 19 02:16 day-10
drwxr-xr-x 1 Ashfaqbs 197121 0 Jan 19 02:16 day-2
drwxr-xr-x 1 Ashfaqbs 197121 0 Jan 19 02:16 day-3
drwxr-xr-x 1 Ashfaqbs 197121 0 Jan 19 02:16 day-4
drwxr-xr-x 1 Ashfaqbs 197121 0 Jan 19 02:16 day-5
drwxr-xr-x 1 Ashfaqbs 197121 0 Jan 19 02:16 day-6
drwxr-xr-x 1 Ashfaqbs 197121 0 Jan 19 02:16 day-7
drwxr-xr-x 1 Ashfaqbs 197121 0 Jan 19 02:16 day-8
drwxr-xr-x 1 Ashfaqbs 197121 0 Jan 19 02:16 day-9
```

Using the above command, we can see the detailed view of a directory or a file

### Creating file

Now, let's see how to create a file. We can use the _touch_ command to write a file.

```sh
 MINGW64 ~/Desktop/10-days-of-code$ touch day-1.txt
 MINGW64 ~/Desktop/10-days-of-code$ ls
day-1  day-1.txt  day-10  day-2  day-3  day-4  day-5  day-6  day-7  day-8  day-9
```

As you can see, there is day-1.txt in the list. That means we have created the day-1.txt file inside the 10-days-of-code folder. You can also you _ls -la_ command to use the detailed view of the folders and file.

### Opening and writing on file

Now, let's open the day-1.txt file and add some text to it. We use the _nano_ command to open and write.

```sh
 MINGW64 ~/Desktop/10-days-of-code$ nano day-1.txt
```

![](/images/nano.png)

As you can see from the above figure, the cursor is active and you can write on the pad. You can only use arrow keys to move the cursor left, right, up, and down. Let's write some text on the opened pad. There are instructors at the bottom that tells how to exit. For instance ctrl + x is to exit. When you exit either you save or cancel which comes when you click ctrl + x.

![](/images/writting_on_nano.png)

Now you can save the modified file by writing Y or you can cancel it by clicking ctrl + c.

After you write Y then click enter.

### Opening file to read

We can use the _cat_ command just only to read the file.

```sh
 MINGW64 ~/Desktop/10-days-of-code$ cat day-1.txt
This is my first text. I have never written on nano text editor before
```

### Copy file

Let's have day-1-backup.txt from day-1.txt by copying using the _cp_ command.

```sh
 MINGW64 ~/Desktop/10-days-of-code
$ cp day-1.txt day-1-backup.txt

 MINGW64 ~/Desktop/10-days-of-code $ ls
day-1  day-1.txt  day-10  day-1-backup.txt  day-2  day-3  day-4  day-5  day-6  day-7  day-8  day-9
```

### Rename file

The _mv_ command is used both to change the name of a file and to move a file into a different directory.

Let's have more files in the 10-days-of-code folder. We can use the _touch_ command to create files.

```sh
 MINGW64 ~/Desktop/10-days-of-code$ touch day-2.txt day-3.txt day-4.txt day-5.txt
 MINGW64 ~/Desktop/10-days-of-code$ ls
day-1      day-10          day-2      day-3      day-4      day-5      day-6  day-8
day-1.txt  day-1-backup.txt  day-2.txt  day-3.txt  day-4.txt  day-5.txt  day-7  day-9
```

Now, let's rename the day-2.txt to second-day.txt using the _mv_ command.

```sh
 MINGW64 ~/Desktop/10-days-of-code$ mv day-2.txt second-day.txt

 MINGW64 ~/Desktop/10-days-of-code$ ls
day-1      day-10          day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9
day-1.txt  day-1-backup.txt  day-3  day-4      day-5      day-6      day-8  second-day.txt

```

Let's rename the day-10 directory to day-ten.

```sh
 MINGW64 ~/Desktop/10-days-of-code$ mv day-10 day-ten
 MINGW64 ~/Desktop/10-days-of-code$ ls
day-1      day-1-backup.txt  day-3      day-4      day-5      day-6  day-8  day-ten
day-1.txt  day-2           day-3.txt  day-4.txt  day-5.txt  day-7  day-9  second-day.txt
```

### Moving file and directory

The _mv_ and _cp_ commands can be used to put files into a directory. The _cp_ moves the copy of the file or the folder to another folder, however, mv just move it without copying.
Let's move the day-1.txt day-1 folder.

```sh
 MINGW64 ~/Desktop/10-days-of-code$ mv day-1.txt day-1
 MINGW64 ~/Desktop/10-days-of-code$ ls
day-1           day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9    second-day.txt
day-1-backup.txt  day-3  day-4      day-5      day-6      day-8  day-ten
 MINGW64 ~/Desktop/10-days-of-code$ cd day-1
 MINGW64 ~/Desktop/10-days-of-code/day-1$ ls
day-1.txt
```

Let's try to move a file using the _cp_ command. Let's move the day-1-backup.txt to day-1 folder

```sh
 MINGW64 ~/Desktop/10-days-of-git/10-days-of-code
$ cp day-1-backup.txt day-1

 MINGW64 ~/Desktop/10-days-of-git/10-days-of-code
$ cd day-1
 MINGW64 ~/Desktop/10-days-of-git/10-days-of-code/day-1
$ ls
day-1.txt  day-1-backup.txt

 MINGW64 ~/Desktop/10-days-of-git/10-days-of-code/day-1
$ cd ..
 MINGW64 ~/Desktop/10-days-of-git/10-days-of-code
$ ls
day-1             day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9    second-day.txt
day-1-backup.txt  day-3  day-4      day-5      day-6      day-8  day-ten
```

The copied version of day-1-backup.txt moved to a day-1 folder.
Now let's create multiple backup files first and move them to a backup folder

```sh
 MINGW64 ~/Desktop/10-days-of-code$ mkdir backups
 MINGW64 ~/Desktop/10-days-of-code$ cd backups
 MINGW64 ~/Desktop/10-days-of-code/backups$ touch day-2-backup.txt day-3-backup.txt
 MINGW64 ~/Desktop/10-days-of-code/backups$ ls
day-2-backup.txt  day-3-backup.txt
```

Moving multiple files

```sh
 MINGW64 ~/Desktop/10-days-of-code
$ mv -t backups day-1-backup.txt day-2-backup.txt  day-3-backup.txt
```

```sh
 MINGW64 ~/Desktop/10-days-of-code
$ cd backups/
 MINGW64 ~/Desktop/10-days-of-code/backups
$ ls
day-1-backup.txt  day-2-backup.txt  day-3-backup.txt
```

### Delete file and directory

Let's remove the file using the _rm_ command. Let's remove the day-1-backup.txt file from the day-1 folder.

```sh
 MINGW64 ~/Desktop/10-days-of-code
$ cd day-1

 MINGW64 ~/Desktop/10-days-of-code/day-1
$ ls
day-1.txt  day-1-backup.txt

 MINGW64 ~/Desktop/10-days-of-code/day-1
$ rm  day-1-backup.txt

 MINGW64 ~/Desktop/10-days-of-code/day-1$ ls
day-1.txt
```

Let's delete the day-ten folder using _rmdir_ command. The _rmdir_ delete a folder.

```sh
 MINGW64 ~/Desktop/10-days-of-code
$ rmdir day-ten

 MINGW64 ~/Desktop/10-days-of-code
$ ls
backups  day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9
day-1    day-3  day-4      day-5      day-6      day-8  second-day.txt
```

Now, let's copy the backups folder to backups-2 and backup-3 using _cp_ command. Then we will delete backups-3. The _cp_ with _-r_ has been used to copy it recursively.

```sh
 MINGW64 ~/Desktop/10-days-of-code$ cp -r backups backups-2

 MINGW64 ~/Desktop/10-days-of-code$ ls
backups    day-1  day-3      day-4      day-5      day-6  day-8  second-day.txt
backups-2  day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9
```

Now let's do the above step to create backups-3

```sh
 MINGW64 ~/Desktop/10-days-of-code
$ cp -r backups backups-3
 MINGW64 ~/Desktop/10-days-of-code
$ ls
backups    backups-3  day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9
backups-2  day-1      day-3  day-4      day-5      day-6      day-8  second-day.txt
```

Now the backups-3 has files and neither the _rm_ nor the _rmdir_ deletes it. Therefore, we can use multiple commands to delete it. Let's try it with the following command.

```sh
 MINGW64 ~/Desktop/10-days-of-code$ rm -rf backups-3
 MINGW64 ~/Desktop/10-days-of-code$ ls
backups    day-1  day-3      day-4      day-5      day-6  day-8  second-day.txt
backups-2  day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9
```

## Git and GitHub

Git is a version control software. In one way or the other you may need to use a git and a GitHub together.

You need to use git and GitHub either to store your projects on the cloud or to collaborate with your team. This means it allows developers or writers to work on the same project even if they are located in different locations.

Version control is a means of recording changes to a file or set of files over time so that you can recall specific versions later.

If you prefer watching the tutorial click this [link](https://www.youtube.com/watch?v=9cCApTLb_Io&list=PLbvhRHYrmshSCAHZbibqh_px_LxnU54dk)

### 1. Install Git

First, you need to install the version control software, Git.

- Git:
  Install [git](https://git-scm.com/downloads)

### 2. Checking status of the repository

The _git status_ command allows you to know the status of the project:
If it is

- initiated
- modified
- staged

We can write the command _git status_ at any time. It is a means to to check what is happening on your project.

### 3. Configure your name and your email

Open the Git bash if your device is Windows, or open the Mac terminal if your device is MacOS and then write the following commands

```shell
git config --global user.name 'yourname'
git config --global user.email 'youremail'
```

### 4. Create a local git repository

In this step, you will create a folder (directory) for your project. A project is just a simple folder that stores all the files related to a certain project. A local repository is a project or a folder that is on your computer.

If your Git bash is not opened, go to start and type git bash. Git terminal will popup on Windows devices. If it is MasOS just open the Mac terminal. On the terminal write:

```shell
mkdir project_name
cd project_name
```

By the way, you can also create the folders the usual way using on the GUI(Graphical User Interface) of Windows or Mac.

### 5. Initialize Git

After creating a new local repository or in an existing local repository, initialize the repository by the following command:

```shell
   git init
```

Once, the repository is initialized git tracks the changes in the files and folders of the project.

### 6. Add file to the staging area

The file can be added to the staging area in multiple ways.
To add a single file, we use the _git add_ command followed by a file name

```shell
   git add filename
```

To add multiple files using their file names using the command _git add_ followed by file names

```shell
   git add filename1 filename2
```

Sometimes, we may make a lot of changes, and adding files one by one is tiring and not product. Therefore, we can use a short and product way. The _git add_ command followed by a dot allows adding files and folders at once to the stage area. Remember, there is a space between the add and the dot.

To add all files and folders at once

```shell
   git add .
```

To add and commit at the same time

```sh
  git commit -am 'commit message'
```

### 7. Unstage a file

```shell
    git reset HEAD filename
```

### 8. Commit the changes

Commit means taking a snapshot or a copy of your file at that point in time. You may associate it with saving a file with a new name (save as).

```shell
   git commit -m 'your message'
```

Your commit message has to be associated with the changes or modifications you make.

### 9. Git log

The _git log_ command allows knowing the commit history of the project. It list down all the commit history

### 10. Git log --oneline

The **git log --oneline** command allows to list minified log history

### 11. Git log -<limit>

For instance, this **git log --5** command list 5 commit history.

### 12. Git check out

We can identify the commit id of each commit using the _git log_ command. Then we can make use of this id to retire any previous commit.

```sh
git checkout commit-id
```

### 13. Creating a branch

We can create a copy of the master(main) using a branch. You built an awesome application. You like to keep this awesome application as it is but you like to add some features.
This is the time, you need branching the master. The branch is the copy of the master at branching instant. After branching, the branch and the master don't see each other. You can create as many branches as you want.

To create a branch:

- Only to create branch

```shell
    git branch  branch-name
```

- To create and checkout to the branch at the same time:

```shell
    git checkout -b branch-name
```

To switch between branches:

```shell
    git checkout main
    git checkout branch-name
```

To list down all the branches:

```shell
    git branch
```

### 14. Create account on GitHub

Now, create an account on GitHub and sign in using your emails and password

- GitHub
  Sign up on [GitHub](https://github.com/)

### 15. Create Repository on GitHub

Go to [GitHub](https://github.com/) and create a repository by click the plus icon on the top right corner.

### 16. Connecting git with remote repository

In this step, you will connect your local git repository with your remote GitHub repository

```shell
    git remote add origin remote_repository_ul
```

The word origin could be any word. It is a means to assign the repository URL.
If this is step is passed without error, you are ready to push it to your remote GitHub repository. Push means actually uploading what you have on your local to remote repository.

### 17. Push

Before you push(upload), please commits any changes and if it is ready push your files to your remote GitHub repository using the following command.

```shell
    git push -u origin master
```

### 18. Merge

When you work on an individual project or a team project you may have different branches. Mostly you will have a master(main), develop and other branches. Then you will merge other branches to your develop and your develop to master. It is possible to merge any branches. For instance, lets merge feature branch to develop

```shell
    git checkout develop
    git merge feature
```

Using the above code, now the develop and feature branches do have the same content

### 19. Pull

If your team merges new features to the develop, then you will be behind, now you need to make your project to the current stage by pulling from develop

```shell
    git checkout yourbranch
    git pull origin develop
```

```sh
    git checkout develop
    git merge yourbranch
    git push -u origin develop
```

If you are a sole developer that works by yourself then you can test the _git pull_ command by modifying some of the files from your remote repository and pull it using the _git pull_ command.

### 20. Git clone

GitHub allows to download a project using a URL. It is the same as downloading by clicking a download button from a website. To clone, go to desktop or any location and write the command _git clone URL_.

For instance, to clone this repository, you need to run the following command

```sh
 MINGW64 ~$ cd Desktop
 MINGW64 ~/Desktop$ git clone https://github.com/Ashfaqbs/10-days-of-git-and-github.git
```

### 21. Rename Branch

To rename a current branch

```sh
git branch -m <newname>
```

To rename any branch

```sh
git branch -m <oldname> <newname>
```

### 22. Deleting Branch

To delete a local branch

```sh
git branch -d branch-name
git branch -D branch-name
```

To delete remote branch

```sh
git push <remote_name> :<branch_name>
```

or

```sh
git push <remote_name> --delete <branch_name>
```

### 23. The .gitignore file

Any file you committed could be pushed to a remote repository but sometimes you may not want to push everything you have on your local repository. For instance sensitive data such as email, password, bank account, API Keys and others. Therefore, any files or folders that is listed on the .ignore file will not be tracked by Git. Create a .ignore file on the top level of your project directory, on this file put file names or folder you would like to ignore

The .ignore file

```sh
test
personal-data
example.txt
sensitive-info.txt
```

### 24 Forking

A forking is a process of owning other repository. After you clicked on fork button of a certain repository you will see that that repository became in your repository list. You can try by clicking the fork button on this repository.

Every repository that has some content in it has an active fork button on the right top corner.
![fork](./images/fork.png)

After forking, we can clone the repository and work on the cloned version of the project. After modifiying the original we can push to the forked verion of the repository. In addition, we can send a pull request to the original repo to contribute on the project.

_Congratulations! Now, you have a solid foundation of Git and GitHub_

## Git cheat sheet:

Here you have the basic git commands which might be useful:

```bash
git --version     # Check the version
git help          # Get help from git
git help commit   # Get help for the commit command
git config        # Get information about configuration
git config --list # Check all what is configured
git config --global user.name "username" # Configuring git user name
git config --global user.email "email"   # Configuring git user email

git init          # Initialize git repository local machine
git status        # Check changes or status of file(s) in repository

git add filename1.txt # Adding only one file
git add filename1.txt filename2.txt # Add multiple files
git add . # Add all the files and folders to the staging area

git commit -a # Stage and write a commit message in Nano
git commit -m "commit message" # Write a commit message after staging
git commit -am "commit message" # Grab everything & skip the stage process

git log  # See the history on the repository
git log --oneline
git log -<limit>
git log --author ="name" # To check change by specific user
git log --graph # Visualize the history

git diff # Compare working copy in the repository
git diff --staged # Compare files in the staging area

git checkout -- filename # To get working copy back
git reset HEAD filename # Removes from the staging area / (unstage)
git checkout <branch-name> <path to file> # Checkout file from different branch
git checkout <commit-id> -- <path to file> # Checkout file from specific commit

git remote -v  # View remote repository-Urls
git remote add <remote name> repository-Url # Add a new remote
git push -u remote master # Push the file into github
git checkout <commit-id> -- filename #

git rm filename1 # Delete one tracked file
git mv filename1 filename2 # Delete tracked file(s)
git mv filename1 foldername/filename1 # Move file to a folder

git branch # to list branches
git branch branch-name # to create a branch
git checkout branch-name # to checkout to a certain branch
git checkout -b branch-name # to create a branch and checkout at the same time
git merge branch-name # to merge a branch to the current branch
```
