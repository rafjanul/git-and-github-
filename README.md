# github_learn
This is a demo repo to learn github
<br>
# Before starting
In Vs code code terminal go to the left side here you will show one + icon from there you can change powershell to gi bash

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
<br>
<h4> structure </h4>
<strong> cd [folder name] </strong>
<br>

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

  
