Git & GitHub Reference
================

### Commands to commit locally and push to GitHub

#### Commit to your local Git:

-    `$ git add . `  "stages" the changed files so they can be "committed"

-    `$ git commit -m "commit message"`  commits staged files to your local repository

#### Push to your remote repository (GitHub):

-    `$ git push origin master` pushes your local master branch to the remote master branch

###### Remember that the *$* is the terminal prompt (do not type the *$*)

-----------------

### Getting started with Git & GitHub - from scratch

###### DO NOT perform these steps if you already have Git set up on your computer...skip to the "Create a new repo" section further down the document

1. Download the Git software from [https://git-scm.com/downloads](git-scm.com)
2. Install the Git software
3. Launch Terminal (on OSX) or Git Bash (on Windows)
4. Navigate to your user folder by issuing this command in the Terminal/Bash prompt

    `$ cd ~` (the *$* is your command prompt - do not type it)

5. Create an SSH key by typing the following command in the Terminal/Bash prompt (just hit the enter key for all prompts except for the email - enter your email when asked)

    `$ ssh-keygen -t rsa`

6. Create an account on [https://www.github.com](github.com)
7. Click your user icon (upper right corner of page) and choose `settings`
8. On the settings page choose `SSH and GPG keys` link
9. Click the `New SSH key` button in the upper right corner of the page
10. Type a title into the Title field - usually the name of your computer
11. Now go back to the Terminal/Bash prompt and export your SSH key with:

    `$ cat ~/.ssh/id_rsa.pub`

12. This should spit out a bunch of numbers and letters - using your cursor, drag-select select them all...from `ssh-rsa` through your email address at the end. Once they are selected hit CMD-C (OSX) or right-click and choose "copy" (Windows)
13. Go back to GitHub and paste (CMD-V/CTRL-V) your key into the "key" field
14. Click on the `Add SSH key` button
15. Now go back to the main GitHub home page (click on the kitty icon in the upper left)
16. Create a "repo" by clicking on the `Start a project` or `New repository` button
17. Name the repository "myfirstrepo", click the "[x] Initialize this with a README" box, and then click the green `Create repository` button
18. You will be taken to the main view of your repo - from here click the green `Clone or download button` and copy the "git@githu..." text
19. Back on your computer, in Terminal/Bash create a folder for all your projects - let's call ours *projects*

    `$ mkdir projects`

20. Let's move into that folder now by typing:

    `$ cd projects`

21. And finally we can now "clone" our repo we just created by typing

    `git clone ` and then CMD-V (OSX) or right-click and choose "paste" (Windows) to paste in the github link

###### You should now have a folder called `myfirstrepo`

-------------

### Creating and cloning a new repo

###### ONLY perform these steps if you have already set up Git on your computer and have made an account on GitHub...see "Getting started with Git & GitHub" section above if you haven't set up git or GitHub yet

15. Sign in to GitHub
16. Create a "repo" by clicking on the `Start a project` or `New repository` button on the main GitHub home page
17. Name the repository, click the "[x] Initialize this with a README" box, and then click the green `Create repository` button
18. You will be taken to the main view of your repo - from here click the green `Clone or download button` and copy the "git@githu..." text
19. Back on your computer, in Terminal/Bash "cd" into your *projects* folder

    `$ cd projects`

21. And then "clone" the repo you just created by typing

    `git clone ` and then CMD-V (OSX) or right-click and choose "paste" (Windows) to paste in the github link

###### You should now have a folder named the same name as your repo

-----------------
