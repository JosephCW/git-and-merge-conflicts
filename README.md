# https-github.com-JosephCW-git-and-merge-conflicts
## Using TortoiseGit, Merge Conflicts, Reverts
### Tortoise Git Example
1. Go to the demo repo and clone the repot onto your machine. 
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/tree/master/resources/TG1.jpg)
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG2.jpg)
2. Next you will create a branch. Right click on the folder the repos in and select "Create Branch". Name it Branch1 and then press ok.
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG3.jpg)
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG4.jpg)
3. Next you will right click the folder again and select "Switch/Checkout...". Then you will select the drop down arrows and choose Branch1. Once you have done that select "OK".
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG5.jpg)
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG4-2.jpg)
4. Open folder and then the txt file and change the top line to any word you want.
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG6.jpg)
5. Right click on the folder the repos in and this time select "Git Commit - Branch1" Once the window opens on the bottom select the drop down arrow and choose "Commit and Push" then select "OK".
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG7.jpg)
6. Right click the folder again and select "Switch/Checkout...". This time you from the drop down arrows choose Master. Once you have done that select "OK".
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG8.jpg)
7. Next you right click the folder and select "Merge". When the window opens make sure that you choose branch and "Branch1" is selected. Once you do that select "OK". This will have merged your "Branch1" with the "Master".
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG9.jpg)
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG10.jpg)
8. You'll notice the txt file is red. Open it up and see the results. You have just created a merge conflict as you are trying to put two different things on the same line.
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG11.jpg)
9. You'll want to remove the head and branch lines so that your left with each item in a different line. When your done it should be simliar to the second image below.
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG12.jpg)
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG13.jpg)
10. Next you will commit again and if a window pops up select ignore.
11. To revert back to a different commit right click the folder again and select "Switch/Checkout.." Choose the "Commit" option and then select the three dots on the right. It should pull up a window simliar to the second image below. From here you can choose to revert back to any commit you wich. Select "Master" and then hit "OK". This will have reverted you back to the orignal file.
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG14.jpg)
![](https://raw.github.com/JosephCW/https-github.com-JosephCW-git-and-merge-conflicts/blob/master/resources/TG15.jpg)









