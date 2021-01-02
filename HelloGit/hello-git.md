# Hello Git
This document will walk through the steps required to get this repository onto your local machine. It will also introduce git and the common commands that will be useful in order to use git.

## What is Git?
Git is a tool for version control. It is used to track changes as they are made to a project. This offers greater control over changes made to a project and provides the ability to roll back to previous revisions if needed. Below is an analogy which should help provide a better picture of how git works.

Imagine you are working on a painting it is going really well and you are happy with it. But then all of the sudden you knock over your black paint over your canvas. 

Your amazing painting seems to be ruined... if only you had a time machine that would take you back to before you spilled that black paint and start working from there again. 

Git provides this for you... while it wont allow you to time travel it does allow you to turn back the clock on the changes you have made to a file. It works by keeping track of the changes that you make. 

Going back to our painting analogy imagine if every time you finished making changes to your painting you took a photo and then uploaded it to a hypothetical time machine. With this "time machine" you could select any image uploaded to it and it would modify your painting to the state it was in in the photo you selected.

This is similar to the manner in which git behaves. YOu can think of git as a tool that will revert your project back into any state that you have "captured an image of" except with git instead of taking actual photos you create commits. 

Commits have messages attached to them which you use to explain what changes you have made. This makes it easier for you to actually point to a specific place you would like to revert to. 

Now imagine you have a friend named Alex who has offered to help you with your painting. You decide Alex should work on adding trees to the painting and you will work on adding a Small barn. The Problem is there isn't a good way for the two of you to work on the canvas at the same time. 

Not to worry though because your nifty "time machine" also has a setting that allows you to pick an image to create a canvas copy of so that both of you can have the exact same canvas to work from to start with. 

This gives you and alex a common place to start from but as you make changes you end up with two different paintings and you need a way to bring the paintings back into one. However, your multi-talented "time machine" still comes through with a solution. 

Each time that you and Alex add new images of your progress to the machine they are combined into the image you started from so your work blends together into one finished product.

This is relatively similar to how branching and merging works within git. You can create multiple branches for different features you are working on in a project and as you add commits to those branches git keeps track of how you are changing from the point that you started. 

Then when you are finished working on the feature branch you can combine that work back into the branch that you started from "intertwining" your changes with any changes that have happened on the starting branch since you diverged from it. 

Now imagine that Alex lives a 12 hour car ride away from you so then they cannot use your nifty "time machine" to get the copy of the painting they need from you. Never fear though because Alex has a painting "time machine" as well and it connects to the internet. 

Your time machine also connects to the internet so you set up a shared folder to pass your photos back and forth. You can download photos from the shared folder onto your "time machine" so you can get a canvas that is updated with the latest changes. 

Each time you make changes to your own canvas you care abel to take a photo, add it to your "time machine" and then upload it to the shared folder.

This is a little bit like how pushes and pulls work in git. Until how all of the operations we have talked about are stored "locally" meaning they can only be tracked by your computer. Pushing and pulling to what is called a "remote repository" allows your changes to be accessible from any computer that has appropriate access. 

When you push your changes that you have created commits for it is like uploading the photos from your "time machine" to a shared folder online. 

When you pull changes from a remote repository it is like downloading the photos from the shared folder to be used on your personal "time machine"

This should provide a high level overview of what exactly git is, but for more learning and information there are a number of great resources that exist and a few of them will be linked at the end of this lesson.

## Getting Started with Git

### Cloning this repository
1. open your terminal and navigate to whatever directory you wish to use for keeping your coding projects. For me I use a directory at the root level of my system named code but it is totally up to personal preference. 
2. once you are in the desired directory run the following command ```git clone https://github.com/annamarieweber/Hello-Code.git``` this performs a clone and will get this repository onto your local machine.

### Creating a branch
1. from your terminal navigate to the project directory using the command ```cd Hello-Code```
2. create a branch to work from using the command ```git checkout -b my-first-branch```

### Making a Change
1. Navigate to the HelloGit.txt file in this directory and add your favorite color to the last line of the file

2. save your changes and then add them to your working tree using the following command ```git add Hello-Code/HelloGit/HelloGit.txt```

3. commit your changes using the command ```git commit -m "hello git"```

4. push your changes using the following command ```git push origin my-first-branch```

### Creating a Pull request


