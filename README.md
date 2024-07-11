# Git3
#Solution of Scenerio 1 : In this we have to make a file project.txt and assume that you and your friend make changes and commit them(change in same line)<br>
We have formed two branches names as "mybranch" and "friendbranch" respectively,and made changes in both branches in same line.<br>
Now,we will first merge friendbranch with main branch using command "git merge friendbranch" when your current working branch is main branch.<br>
Now when we try to merge another mybranch with main an conflict occurs named as "MERGED CONFLICT" which occurs when user make diffrent changes to same line of the same file.<br>
Here is scrrenshot of MERGE CONFLICT : ![alt text](<merge conlict ss.jpg>)                      <br>
Now,we will resolve the conflict manually with an expected reult i.e  Changes from both branches should be included in the file in the main branch. The changes should be included in the sequence: first your teammate’s changes and then the changes made by you.<br>
Here is scrrenshot of Resolved merge conflict: ![alt text](<ss of solved merge conflict.jpg>)           <br>
Command used: 1.git checkout -b branchname = It create new branch <br>
              2.git checkout branchname = used to change branch <br>
              3.git branch = shows the present branch <br>
              4.git merge branchname = merge the branchname with current branch. 
        <br>
<br>
#Solution of  Scenerio 2 :In this we have to  Add Files and Commit Together <br>
First we will form file "index.html","file.txt" and add all files to the staging area using command "git add ." and commit them with a "single command :git commit -m "All files are added"<br>
Here is screenshot of this: ![alt text](<ss second scenerio.jpg>)     <br>
Now we will Verify the commit by checking the "commit log" command.<br>
Here is screenshot of verification: ![alt text](<ss verification second.jpg>)    <br>
Command used:1.git add . = it adds a change in the working directory to the staging area <br>
            2.git commit = it commit the changes to the stagigng area <br>
            3.git log = Verify the all commits are done.
            <br>
            <br>
 #Solution of Scenario 3:In this we have to Include Additional Commit in the Previous Commit Message.<br>
 First we will create a file names as "initial file"abd commit changes using git commit command.Now,we will do some changes and then Stage the changes and amend the last commit using command "git commit --amend --no-edit"<br>
Here is screenshot of amend command :![alt text](<amend ss.jpg>)   <br>
Next we will Verify the amended commit by checking the commit log <br>
Here is screenshot of verification:![alt text](<ss verify 3rd.jpg>)    <br>
Used Command : 1. git commit -m "some message" = commit the changes <br>
               2. git commit --amend --no-edit = It amends the previous commit.<br>
               3. git log = Verify the all commits are done.<br>
               <br>
               <br>
#Solution of Scenario 4: In this we have to use Stash Command when we are working on a feature but need to quickly switch to another task without committing your current changes.  <br>
In this first we will Make changes to a file but do not commit them and use an stash command to save directory and index state to work upon next branch without commiting previous one.<br>
Here is screenshot of stash command :![alt text](<ss stash .jpg>)   <br>
Now,we will Verify that your working directory is clean that can be seen in previous command.<br>
Apply the stashed changes back using command "git stash apply" to revert back the stash command<br>
Here is screenshot of stash apply command :  ![alt text](<ss stash apply.jpg>)    <br>
Command used : 1.git stash = temporarily stashes changes you have made to your working copy so you can work on something else,and then come back and re-apply them later on.<br>
               2.git stash apply = reverts the stash command <br>
               3.git list = it will pull up a list of your repository stashes.<br>
               4.git pop = it removes or throws away the latest or the topmost stash.<br>
               <br>
               <br>
#Solution of Scenario 5: Use of .gitignore










#Solution of Scenario 6:Revert to Previous Commits <br>
We will do this when You made a mistake in a recent commit and need to revert the changes. <br>
First we will  Create a file and commit changes to the file using commit command and then Make another commit with a mistake and then Revert to the previous commit, undoing the mistake using revert command "git reset HEAD~1"<br>
Here is screenshot of revert command :  ![alt text](<ss scenerio6.jpg>)    <br>
Here is screenshot of verification of state :![alt text](<ss scenerio6.jpg>)
<br>
then we will Verify the state of the repository to ensure the revert was successful using git status command. <br>
Command Used : 1.git commit -m "some message" = commit the changes <br>
               2.git reset HEAD~1 :used to Revert to the previous commit<br>
               3.git status : display the state of the working directory and the staging area<br>
               <br>
               <br>
#Solution of Scenario 7: Create a Pull Request when you have made changes on a feature branch and want to merge them into the main branch via a pull request. <br>
First we will Create a new branch from the main branch and make changes and then Push the branch to the remote repository using "git checkout -b branchname " and "push origin branchname(feature).<br>
Now,Create a pull request to merge your feature branch into the main branch.<br>
In this way of merging an branch with main by pulling request file changed and oe commit is made in github.We have merged the feature branch using github not git bash.Using this it enables developers to make a new features or kill bugs without altering the project main code or what the user see.<br>
Here are the screenshot of changes :![alt text](<ss change1.jpg>) ,![alt text](<ss change2.jpg>), ![alt text](<ss change3.jpg>)   <br>
Command used : 1.git checkout -b branchname = It create new branch <br>
               2.push origin feature = it will push commited changes from local to remote repository.<br>
