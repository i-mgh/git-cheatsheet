# git-cheatsheet
Dwsclassdws-dev-1- Exercise Solving Exercise 4 
Objective: Education about GIT
How to use: Read related questions and answers
Collaboration: Please send your comments to my email mohsen@ghadamyari.net

1) Why do we use version control tools like GIT?
GIT is the most common version control system in the world for tracking text file changes. GIT gives us the ability to control files and provide information on how to change files. That is, in a change made to a file, it can say exactly what has changed and who made it, and when. Using the gate, we can manage and control the process of updating and changes in project files among programmers during the project time.

2) What important files does a good repository have?
A repository is a place for storing project-related code and change history.
A good repository must have README, .gitignore, and license files.

3) What are the parts of a good document?
A good document should have the following sections:
1) The purpose of the project
2) How to use the project
3) How to collaborate with the project.

4) What does the 'git clone' command do?
To clone a remote repository into a local repository

5) If we want to update the local repository with the repository remote, what command should be executed?
git pull

6) What is the difference between 'reset', 'revert', 'checkout'?
reset: Reset the current HEAD to the specified state
revert: Sometimes we have to undo the changes we have made. One surefire way to get it back is to use git revert.
checkout: Often used to move from one branch to another.

7) What is the difference between 'merge' and 'rebase'?
'merge' and 'rebase' both merge the changes made in the subdirectories to the main directory, but differ in how they merge. 'merge' creates a new commit by merging and preserves directory history. By merging the branch commits with the main branch, 'rebase' removes duplicate commits and maintains only one branch and path throughout the project, and no new commits are generated as a result of this merge.

8) What command is used to view the history of commits?
git log

9) What command do we use if we want to see changes of a file?
git deff

10) What is the use of a tag? How to create a tag?
The tag is used for versioning and tagging specific points of the project as important points.
GIT supports two types of tags: lightweight and annotated:
The lightweight tag is just a simple tag, but annotated information including the name and email of the tagger, tagging time, relevant committees, etc. is also stored.
The following command can be used to tag:

**lightweight:**
git tag v1.1
 
**annotated:**
git tag -a v1.1 -m  “version 1.1”

11) What is the process to participate in a project that is managed with a GIT?
We prepare a directory in the system with the 'git init' command. Then we create a clone on our system from the desired repository with the 'git clone' command.
We create a branch for the changes we want to make.
We write our code on the created brunch and whenever the added commands are ready to commit, after being added to the stage by 'git add', we commit them with the 'git commit' command.
Finally, we push it to transfer the local branch to the remote branch with 'git push' command.

12) What are the branches used for and how can they be integrated?
We use brunch to add a new feature to the program or fix existing bugs.
Suppose a search brunch is created to add the search feature. We use one of the following methods to integrate:

git checkout master
git merge master search

Or, another way to integrate branches is to use rebase:

git checkout master
git rebase master search
