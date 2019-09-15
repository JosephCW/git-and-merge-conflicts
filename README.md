# Using TortoiseGit, Merge Conflicts, Reverts

## Tortoise Git Example

1. Go to the demo repo and clone the repot onto your machine.
![](resources/TG1.png)
![](resources/TG2.png)
2. Next you will create a branch. Right click on the folder the repos in and select "Create Branch". Name it Branch1 and then press ok.
![](resources/TG3.png)
![](resources/TG4.png)
3. Next you will right click the folder again and select "Switch/Checkout...". Then you will select the drop down arrows and choose Branch1. Once you have done that select "OK".
![](resources/TG5.png)
![](resources/TG4-2.png)
4. Open folder and then the txt file and change the top line to any word you want.
![](resources/TG6.png)
5. Right click on the folder the repos in and this time select "Git Commit - Branch1" Once the window opens on the bottom select the drop down arrow and choose "Commit and Push" then select "OK".
![](resources/TG7.png)
6. Right click the folder again and select "Switch/Checkout...". This time you from the drop down arrows choose Master. Once you have done that select "OK".
![](resources/TG8.png)
7. Next you right click the folder and select "Merge". When the window opens make sure that you choose branch and "Branch1" is selected. Once you do that select "OK". This will have merged your "Branch1" with the "Master".
![](resources/TG9.png)
![](resources/TG10.png)
8. You'll notice the txt file is red. Open it up and see the results. You have just created a merge conflict as you are trying to put two different things on the same line.
![](resources/TG11.png)
9. You'll want to remove the head and branch lines so that your left with each item in a different line. When your done it should be simliar to the second image below.
![](resources/TG12.png)
![](resources/TG13.png)
10. Next you will commit again and if a window pops up select ignore.
11. To revert back to a different commit right click the folder again and select "Switch/Checkout.." Choose the "Commit" option and then select the three dots on the right. It should pull up a window simliar to the second image below. From here you can choose to revert back to any commit you wich. Select "Master" and then hit "OK". This will have reverted you back to the orignal file.
![](resources/TG14.png)
![](resources/TG15.png)

## Git Bash Example

1. Create a new repository on your github account and then clone the repo with 'git clone \<Repository Url>'
![](resources/GB1.png)
2. Create a new text file and then add and commit the changes. Tortoise Git does both the staging of files and the committing in one step, but Git Bash does these two steps independently. Following standard unix style file paths one can stage a file to be committed using the 'git add \<Path / File Name>' command. After adding you can verify what was added using the 'git status' command. Now that the file changes are staged and ready to be committed, go ahead and commit it using the 'git commit -m "\<Message Here>"' command.
2. Create a new branch with the command 'git branch \<New Branch Name>', then check out the new branch using the command 'git checkout \<New Branch Name>'. This can also be achieved in one step by using 'git checkout -b \<New Branch Name>'.
![](resources/GB5.png)
3. Make some changes to the text.txt file and then commit. (No need to push)
![](resources/GB4.png)
4. At this point go ahead and switch back to the master branch by running 'git checkout master'. Make a change to the text.txt file and make another commit after staging the file.
![](resources/GB6.png)
5. One of the key differences between git and other SCM tools is that it allows you to have an entire separate copy of the project on your local machine and to work with branches all without effecting the copy that others are working with. Unfortunately a somewhat common biproduct of this process when two people are working on a related part of a program is a merge conflict. By being on the branch that you want the changes merged into, run the 'git merge \<Other Branch>' command.
![](resources/GB7.png)
6. As described above, git is unsure of how to handle multiple changes to the same line of a file. In order to 'help' the situation, git will put angle brackets and hyphens to separate the content it is unsure of.
![](resources/GB8.png)
7. Once you have manually modified the file to look the way that you believe is fit, go ahead and stage the files and then commit again. Congratulations, you've just solved a merge conflict!
![](resources/GB9.png)
