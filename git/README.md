# General

What is source code management
What is Git
What is GitHub
What is the difference between Git and GitHub
How to create a repository
What is a README
How to write good READMEs
How to commit
How to write helpful commit messages
How to push code
How to pull updates
How to create a branch
How to merge branches
How to work as collaborators on a project
Which files should and which files should not appear in your repo

# Tasks

0. Create and setup your Git and GitHub account

Step 0 - Create an account on GitHub
You will need a GitHub account for all your projects. You can create an account for free here

Step 1 - Create a Personal Access Token on Github
To have access to your repositories and authenticate yourself, you need to create a Personal Access Token on Github.

You can follow this tutorial to create a token.

Once it’s created, you should have a token that looks like this:

Step 2 - Update your profile on the Intranet
Update your Intranet profile by adding your Github username here

If it’s not done the Checker won’t be able to correct your work

Step 3 - Create your first repository
Using the graphic interface on the github website, create your first repository.

Name: Look at the bottom of the project to see the name of the repository
Description: This is my first repository as an ALX learner
Public repo
Ignore the options relating to README, .gitignore, or license

Step 4 - Open the sandbox / text editor
On the intranet, just under the task, click on the button and run to start the machine.

Once the container is started, click on to open a shell where you can start work from.

Using a different text editor (eg: Visual studio code): Open the text editor and access the terminal in that text editor. In vs code you can use the keyboard shortcut CTRL + ` to open the in built terminal.

Step 5 - Clone your repository
On the webterm of the sandbox or the terminal of your chosen text editor, do the following:

Clone your repository

root@896cf839cf9a:/# git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/{YOUR_REPO}.git  
Cloning into '{YOUR_REPO}'...
warning: You appear to have cloned an empty repository.

Replace {YOUR_PERSONAL_TOKEN} with your token from step 1

Replace {YOUR_USERNAME} with your username from step 0 and 1

Replace {YOUR_REPO} with the name of the reposotiry at the bottom of the task

Step 6 - Create the README.md and push the modifications
Navigate to this new directory. Tips

root@896cf839cf9a:/# cd {YOUR_REPO}/
root@896cf839cf9a:/{YOUR_REPO}#

Create the file README.md with the content My first readme. Tips

root@896cf839cf9a:/{YOUR_REPO}# echo 'My first readme' > README.md  
root@896cf839cf9a:/{YOUR_REPO}# cat README.md  
My first readme  
Add this new file to git, commit the change with this message “My first commit” and push to the remote server / origin
root@896cf839cf9a:/{YOUR_REPO}# git add .
root@896cf839cf9a:/{YOUR_REPO}# git commit -m 'My first commit'
[master (root-commit) 98eef93] My first commit
1 file changed, 1 insertion(+)
create mode 100644 README.md
root@896cf839cf9a:/{YOUR_REPO}# git push  
Enumerating objects: 3, done.  
Counting objects: 100% (3/3), done.  
Writing objects: 100% (3/3), 212 bytes | 212.00 KiB/s, done.  
Total 3 (delta 0), reused 0 (delta 0)  
To https://github.com/{YOUR_USERNAME}/{YOUR_REPO}.git

- [new branch] master -> master  
  Good job!

You pushed your first file in your first repository.

You can now check your repository on GitHub to see if everything is good.

1. Repo-session

Create a new directory called git in your repository.

Make sure you include a non-empty README.md in this new directory.

2. Coding fury road

For the moment we have an empty project directory containing only a README.md. It’s time to code!

Create these directories at the root of your project: html, css, js
Create these empty files:
home.html in the html directory
main.js in the js directory
style.css in the css directory
Create a file alx.js in the js directory with this one line inside: console.log("ALX")
Create a file school.js in the js with this one line inside: console.log("School")
Add all these new files to git
Commit your changes (message: “Starting to code today, so cool”) and push to the remote server
