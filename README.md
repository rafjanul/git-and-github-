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
<br>
<h4> structure </h4>
<strong> ls </strong>
<br>
<h4> To view the hidden folders</h4>
<strong> ls -a </strong>
<br>

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

# To check the branch
it is used to check in which branch we are
<h4> structure </h4>
<strong> git branch </strong>

# To rename any branch
it is used to rename any branch 
<h4> structure </h4>
<strong> git branch -M [new name] </strong>





  
