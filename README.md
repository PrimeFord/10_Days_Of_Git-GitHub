# 10_Days_Of_Git-GitHub

This respository is a summarized version of 10 Days of Git & GitHub by Aabeneh Yetayeh.

## Git codes

### Current working directory

Checking the working directory using the command _pwd_.

### Navigating directory

Now, let's go to the Desktop using _cd_ (change directory).

### Making Directory

Now, let's create a directory inside the Desktop. Call the name of the directory, 10-days-of-code. You give it any name but I am in favor of this name. Use the _mkdir_ command to make a directory(folder)

### List files and directories

We can check the files and directories we have in a directory(folder) using the _ls_ command.

### Detail list

Let's see a detailed list of the directories using multiple commands, _ls -la_.

### Creating file

Now, let's see how to create a file. We can use the _touch_ command to write a file.

### Opening and writing on file

Now, let's open a file and add some text to it. We use the _nano_ command to open and write.

### Opening file to read

We can use the _cat_ command just only to read the file.

### Copy file

Using the _cp_ command.

### Rename file

The _mv_ command is used both to change the name of a file and to move a file into a different directory.

### Moving file and directory

The _mv_ and _cp_ commands can be used to put files into a directory. The cp moves the copy of the file or the folder to another folder, however, mv just move it without copying.

Moving multiple files _mv -t folder file1 file2_

### Delete file and directory

Let's remove the file using the _rm_ command. Let's remove the day-1-backup.txt file from the day-1 folder.

Let's delete the day-ten folder using rmdir command. The _rmdir_ delete a folder.

If a folder has files in it, neither the rm nor the rmdir deletes it. Therefore, we can use multiple commands to delete it. Let's try it with the following command _rm -rf foler with files_

## Github codes

git --version # Check the version
git help # Get help from git
git help commit # Get help for the commit command
git config # Get information about configuration
git config --list # Check all what is configured
git config --global user.name "username" # Configuring git user name
git config --global user.email "email" # Configuring git user email

git init # Initialize git repository local machine
git status # Check changes or status of file(s) in repository

git add filename1.txt # Adding only one file
git add filename1.txt filename2.txt # Add multiple files
git add . # Add all the files and folders to the staging area

git commit -a # Stage and write a commit message in Nano
git commit -m "commit message" # Write a commit message after staging
git commit -am "commit message" # Grab everything & skip the stage process

git log # See the history on the repository
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

git remote -v # View remote repository-Urls
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
