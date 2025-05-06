something is wrong with these instructions:

https://docs.github.com/en/get-started/using-git/about-git

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
git push --set-upstream origin main

check this out:

bjanu@MSI MINGW64 ~/desktop/gitgoing
$ git init
Initialized empty Git repository in C:/Users/bjanu/Desktop/gitgoing/.git/

bjanu@MSI MINGW64 ~/desktop/gitgoing (master)
$ touch README.md

bjanu@MSI MINGW64 ~/desktop/gitgoing (master)
$ git add README.md

bjanu@MSI MINGW64 ~/desktop/gitgoing (master)
$ git commit -m "add README to initial commit"
[master (root-commit) 9f17139] add README to initial commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md

bjanu@MSI MINGW64 ~/desktop/gitgoing (master)
$ git status
On branch master
nothing to commit, working tree clean

bjanu@MSI MINGW64 ~/desktop/gitgoing (master)
$ git remote add origin https://github.com/bjanusek00/gitgoing.git

bjanu@MSI MINGW64 ~/desktop/gitgoing (master)
$ git push --set-upstream origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/bjanusek00/gitgoing.git'

bjanu@MSI MINGW64 ~/desktop/gitgoing (master)
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/bjanusek00/gitgoing.git'

bjanu@MSI MINGW64 ~/desktop/gitgoing (master)
$ git push --set-upstream origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/bjanusek00/gitgoing.git'

bjanu@MSI MINGW64 ~/desktop/gitgoing (master)
$ git branch -M main

bjanu@MSI MINGW64 ~/desktop/gitgoing (main)
$ git remote add origin https://github.com/bjanusek00/gitgoing.git
error: remote origin already exists.

bjanu@MSI MINGW64 ~/desktop/gitgoing (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 238 bytes | 238.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/bjanusek00/gitgoing.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

bjanu@MSI MINGW64 ~/desktop/gitgoing (main)
$
