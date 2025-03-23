# Purpose of the Exercise
This exercise is designed to help you understand how to use Git's stash feature, which allows you to temporarily save changes that you are not ready to commit. This is useful when you need to switch branches or work on something else without losing your current work. Understanding how to stash and pop changes is essential for managing your workflow effectively.

## Conclusion
By completing this exercise, you have learned how to create new files, stash changes, and restore them using Git's stash feature. This is a valuable skill for managing your workflow, especially when you need to switch contexts or work on multiple features simultaneously. Understanding how to use stashing effectively can help you maintain a clean and organized codebase while allowing you to work flexibly.


# Steps to Complete the Exercise

1. Create a New home.html File, Add Some HTML Changes, and Save Them

In your project folder, create a new file named home.html.
Add some basic HTML content to home.html and save the file.
2. Stash Save Your Current Changes

Open the terminal in VS Code.
Stash your changes:


- git stash save "Add home.html"

3. Repeat the Same Process for a New about.html Page and Stash Save Your Changes

Create a new file named about.html.
Add some HTML content to about.html and save the file.
Stash your changes:
- git stash save "Add about.html"
  
4. Repeat the Same Process for a New team.html Page and Stash Save Your Changes

Create a new file named team.html.
Add some HTML content to team.html and save the file.
Stash your changes:

- git stash save "Add team.html"

5. Using Stash Pop Restore the Changes of the about.html Page

Pop the stash for the about.html changes:
- git stash pop stash@{1}

Note: The index may vary based on how many stashes you have. You can check your stash list with:

- git stash list
  
6. With the Help of an Index Use Stash Pop Bring Back the home.html Page Changes

Pop the stash for the home.html changes:

- git stash pop stash@{2}

7. Commit the Current Changes and Push Them

Stage your changes:

- git add .
  
Commit your changes:

- git commit -m "Add home and about pages"

Push your changes to GitHub:


- git push origin main

8. Using Stash Pop Restore the Changes of the team.html Page Index

Copy code
git stash pop stash@{0}
Reset the Current Changes Using Git Reset and Go Back to the Changes Without the team.html Page

1. Reset your changes to the last commit, excluding the team.html changes:

- git reset HEAD~1

This command will reset your working directory to the last commit, but since you have already popped the team.html changes, it will remove those changes from your working directory.


# Stashing
## Def
    is super useful command that helps you save changes that you are not yet ready to commit. You can stash changes and then come back to them later.
## git stash
    Running git stash will take all uncommitted changes (staged and unstaged) and stash them , reverting the changes in your working copy 
    > git stash  / you can also use git stash save instead 

    This command applies the most recent stashed changes to your working directory and then removes that stash from the stash list. It’s a quick way to apply and clean up.

## git stash pop
    Use git stash pop to remove the most recently stashed changed and re-apply them to your working copy and if you do not only need the recent stashed one you can just write ## git stash pop "stash-id"

    Similar to git stash pop, this command applies a specific stash (in this case, the one identified as stash@{1}) to your working directory and then removes that specific stash from the list.

## git Stash Apply
    you can use git stash apply to apply whatever is stashed away, without removing it from the stash. This can be useful if you want to apply stashed changes to multiple branches.

    This command applies the most recent stashed changes to your working directory, but does not remove the stash from the stash list. It leaves the stash available for later use.

## git stash -u
    If you have untracked files(Files that you have never checked in to Git), they will not be incuded in the stash

    Fortunately, you use the -u option to tell git stash to include those untracked files. 
## git stash list
    By running it , the stashed list will be showed
## git stash apply stash@{2}
git assumes you want to appy the most recent stash when you run git stash apply stasht@{2}

When you stash changes to example.txt multiple times, each stash is assigned a unique ID (e.g., stash@{0}, stash@{1}), reflecting the state of the file at different points. Consequently, the newer stash will include all previous changes along with any new edits made after applying the earlier stash.

## git stash drop "stash@{2}"

    To delete a particular stash, you can use git stash drop @<stash-id>

## git stash clear
     it is used to clear out all stashes, run git stash clear

     This command removes all stashed changes from the stash list. It is a way to clean up your stash entirely, and it can't be undone.