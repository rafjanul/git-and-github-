# github_learn
This is a demo repo to learn github

# Before starting
In Vs code code terminal go to the left side here you will show one + icon from there you can change powershell to gi bash (optional)

# Clone a github repo in our local machine
<h4> structure </h4>
<strong> git clone [url] </strong>
<br>
retrieve an entire repository from a hosted location via URL
<br> 

# Use of change directory
cd means change directory
<br>
the use of cd is suppose if we want to go from an outside folder to an inside folder we use that
<h4> structure </h4>
<strong> cd [folder name] </strong>
<br>

now suppose we want to come outside of a folder for this we use
<h4> structure </h4>
<strong> cd .. </strong>

# Use of mkdir
it is used to create a new folder
<h4> structure </h4>
<strong> mkdir [folder name] </strong>


# Use of list files
ls means list files
<br>
the use of ls is that if we want to see all the files in a folder we use that
<h4> structure </h4>
<strong> ls </strong>
<h4> To view the hidden folders</h4>
<strong> ls -a </strong>

# Display the status of the files
<h4> structure </h4>
<strong> git status </strong> 
<br>
show modified files in working directory, staged for your next commit
<br> 
basically it means whatever code is in github is in the vs code (code editor)

<h2> What happens when the status is not the same</h2>
<h3> In that case the following four conditions arises </h3>

<ol>
  <li> <h4> untracked </h4> </li>
  new files that git doesn't yet track (files created in code editor not uploaded to git)
  
  <li> <h4> modified </h4> </li>
  changed
  
  <li> <h4> staged </h4> </li>
  file is ready to be committed
  
  <li> <h4> unmodified </h4> </li>
  unchanged  
</ol>

<h2> How to add the file and actually commit</h2>
<h3> There are two steps to that </h3>
<ol>
  <li> <h4> add </h4> </li>
  adds new or changed files in your working directory to the git staging area
  <h4> structure </h4>
<strong> git add [file name] </strong>
  <br>
  or
  <br>
  <strong> git add . </strong> {this means to add all the changes instead of writing individual file names}
<br>
  <li> <h4> commit </h4> </li>
  it is the record of the change (the confirmation that the change happened)
  <h4> structure </h4>
<strong> git commit-m "[any message]" </strong> 
</ol>

# Use of push
it is used to push the changes we added and committed in our local machine to github
<h4> structure </h4>
<strong> git push [alias] [branch] </strong>
<br>
in this case it will be
<br>
<strong> git push origin main </strong> 

<h4>also to push a lot of changes</h4>
<strong>git push -u origin main </strong>
<br>
after that we can just use <strong>git push </strong> to push the changes

# Create repo from our local machine 
for this we use the <strong> init </strong> command
<br>
it is used to create a new git repo 
<h4> structure </h4>
<strong> git init </strong>

# Adding a new remote repo 
it is used to add a new git remote repo 
<h4> structure </h4>
<strong> git remote add origin [url] </strong>

# Verify the remote
<h4> structure </h4>
<strong> git remote -v </strong>

# Branch
it is like a tree branch. if we make any changes in one branch it won't show in other branch

# To check the branch
it is used to check in which branch we are and also list all the branches 
<h4> structure </h4>
<strong> git branch </strong>

# To rename any branch
it is used to rename any branch 
<h4> structure </h4>
<strong> git branch -M [new name] </strong>

# To move to another branch
it is used to move to any branch 
<h4> structure </h4>
<strong> git checkout [branch name] </strong>

# To create a new branch
it is used to create a new branch 
<h4> structure </h4>
<strong> git checkout -b [new branch name] </strong>

# To delete a branch
it is used to delete any branch 
<h4> structure </h4>
<strong> git branch -d [branch name] </strong>
<br>
<h4>
 a note: if we are trying to delete a branch in which we are currently in it will show error as it can't be done 
</h4>

# Comparing and checking difference between two branches
suppose i made a change in a branch now i want to see and compare it with the other branches.
<h4> structure </h4>
<strong> git diff [branch name that we are trying to compare with] </strong>

# Merge Branches
it is used to merge various separate branches 
<h4> There are two ways to do it </h4>
<ol>
  <li> Way-1 [via local machine] </li>
  <h4> check the difference </h4>
  <strong>git diff [branch name] </strong>
  <h4> Merge </h4>
  <strong>git merge [branch name] </strong>

  <li> Way-2 [via github] </li>
  <strong> Create a pull request </strong>
  <br>
  pull request lets you tell others about the changes you've pushed to a branch in a repository on Github  
</ol>

# Update the merge from remote repo to local machine
suppose we merged the branch using the pull request but it still won't show on the local machine so for this we will need to use a command.
<h4> structure </h4>
<strong> git pull origin main </strong>
<br>
it is used to fetch and download content from a remote repo and immediately update the local repo to match the content

# Merge conflict
suppose in a two branch a line is changed in the exact same positon
<br>
example: this is a feature -> old (in main branch) 
<br>
this is a feature (button) -> updated (in main branch)
<br>
this is a feature (dropdown) -> updated (in a new branch)
<br> 
now if we try to merge that new branch with the main branch it will create a conflict 
<br>
to solve this in vs code we will see various options (1. accept incoming change, 2. accept current change, 3. accept both change) we can solve it by clicking any of the options

# Showing the commit history
<h4> structure </h4>
<strong> git log </strong>
<br>
show the commit history for the currently active branch

# Undoing changes
suppose we made changes that we regret now how to do that
<ol>
  <li> <h3> Staged changes </h4> </li>
  these are changes that have been added but are yet to be committed
  <h4> structure </h4>
  <strong> git reset [file name] </strong>
  <br>
  or
  <br>
  <strong> git reset </strong> {this means to reset all the changes instead of writing individual file names}

  <li> <h3> Committed changes [to go back one commit] </li> </h3>
  changes that are mistakenly committed
  <h4> structure </h4>
  <strong> git reset HEAD~1 </strong>
  <br>
  HEAD -> this means the last commit we did
  <br>
  ~1 -> this means to change back one step

  <li> <h3> Committed changes [to go back multiple commits] </li> </h3>
  <h4> structure </h4>
  <strong> git reset [hash of that commit (can be seen using log)] </strong>
  <br> 
  the changes is now gone from git but to remove it from the local machine we need to use another command
  <h4> structure </h4>
  <strong> git reset --hard [hash of that commit (can be seen using log)] </strong>
  <br>
  it will remove the changes from both git and the code editor

</ol>

# Fork
A fork is a new repository that shares code and visibility settings with the original 'upstream' repository
<br>
Fork is a rough copy