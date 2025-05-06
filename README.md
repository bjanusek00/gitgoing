https://docs.github.com/en/get-started/using-git/about-git
something is wrong w these instructions:

Example: Start a new repository and publish it to GitHub
First, you will need to create a new repository on GitHub. For more information, see Hello World. Do not initialize the repository with a README, .gitignore or License file. This empty repository will await your code.

# create a new directory, and initialize it with git-specific functions
git init my-repo

# change into the `my-repo` directory
cd my-repo

# create the first file in the project
touch README.md

# git isn't aware of the file, stage it
git add README.md

# take a snapshot of the staging area
git commit -m "add README to initial commit"

# provide the path for the repository you created on github
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY-NAME.git

# push changes to github
~~git push --set-upstream origin main~~
$ git branch -M main

$ git push -u origin main

Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 238 bytes | 238.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/bjanusek00/gitgoing.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

![image](https://github.com/user-attachments/assets/9115330f-51e4-469b-ba94-297d89855f79)
