Purpose of the Exercise
This exercise is designed to familiarize you with basic Git and GitHub operations, which are essential for version control and collaborative software development. Understanding these concepts is crucial because:

Version Control: Git allows you to track changes in your code, making it easier to manage different versions of your project.
Collaboration: GitHub provides a platform for multiple developers to work on the same project simultaneously, facilitating collaboration.
Branching: Branches allow you to work on features or fixes in isolation without affecting the main codebase, which is vital for maintaining a stable project.
Steps to Complete the Exercise
Create a Project Folder & Initialize Git

Open VS Code.
Create a new folder for your project (e.g., my-project).
Open the terminal in VS Code (View > Terminal).
Navigate to your project folder:
bash
Run
Copy code
cd path/to/my-project
Initialize a Git repository:
bash
Run
Copy code
git init
Make Changes to the Project (Add Files and Contents)

Create a new file (e.g., index.html) in your project folder and add some basic HTML content.
You can also create a README.md file to describe your project.
Rename Your Main Branch from master to main

Check your current branch name:
bash
Run
Copy code
git branch
If your branch is master, rename it to main:
bash
Run
Copy code
git branch -m master main
If it’s already main, rename it to master and then back to main:
bash
Run
Copy code
git branch -m main master
git branch -m master main
Stage Your Changes and Commit Them

Stage your changes:
bash
Run
Copy code
git add .
Commit your changes:
bash
Run
Copy code
git commit -m "Initial commit"
Create a GitHub Repo and Connect It with Your Project

Go to GitHub and create a new repository (e.g., my-project).
Follow the instructions provided by GitHub to connect your local repository to the remote one. Typically, it looks like this:
bash
Run
Copy code
git remote add origin https://github.com/yourusername/my-project.git
Push Your Changes to GitHub

Push your changes to the main branch on GitHub:
bash
Run
Copy code
git push -u origin main
Create a New Branch dev

Create and switch to a new branch called dev:
bash
Run
Copy code
git checkout -b dev
From dev, Create Another Branch test

Create and switch to a new branch called test from dev:
bash
Run
Copy code
git checkout -b test
Go Back to the dev Branch and Delete the test Branch

Switch back to the dev branch:
bash
Run
Copy code
git checkout dev
Delete the test branch:
bash
Run
Copy code
git branch -d test
Conclusion
By completing this exercise, you have learned how to initialize a Git repository, manage branches, and push your code to GitHub. These skills are fundamental for any developer working on collaborative projects or maintaining their own codebases. Understanding Git and GitHub will help you manage your projects more effectively and collaborate with others in the software development community.