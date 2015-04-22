Now that we have cloned this repository, if we look at the Repository Browser window we will see an entry for that repository.

Now I will close the Repository Browser.

Now I will add a file to that repository using my text editor of choice and make some changes to an existing file. This repository includes a guest list file in the lesson 4 folder. You can add your name to that if you'd like. Once you learn to submit a pull request, maybe we will add your request to the original repository.

Now I will go back to SourceTree with the "git-learning" repository screen showing. The commit history has the most recent item at the top and above that is an entry labelled "Uncommitted changes". Select that and you will get detail showing the file or files you have changed, added, or deleted.

Below the commit history section of the screen you will see the names of these files. Changed files will have a yellowish orb next to them and new files will have a question mark icon next to them. When you click on a filename you will see detail showing the changes to changed files and the entire file for new files.

Notice the checkboxes to the left of the filenames. Checking the boxes indicates that you want to perform some action on the files. Usually new files are not automatically checked and changed files are. For now, make sure all of the boxes are checked. Up to this point you have already used the Git "status" command because SourceTree shows you the new and changed files.

Now click the "Commit" option in the toolbar. At the bottom of the screen you will now see an area where you can type the message for the commit. Remember that the first line should be 50 characters or less and should be considered the subject of this revision. SourceTree does not impose any limits on the text, but when the message shows up in GitHub.com the 1st line will be truncated and put in a subject-like field with the remainder of that line and the other lines in another text box.

Type your commit, or revision, message and click commit. The first time you select new files and click "Commit", SourceTree will ask you to confirm the addition of the new files. It will also do the same for deleted files. If you do not want to be asked again, check the checkbox, and then click "OK". Otherwise, just click "OK".

At this point you have just used the Git "add" and "commit" commands. Now you will notice that the "Uncommitted changes" phrase has been replaced with the revision represented by part of your commit message.

Remember that at this point the changes are still just on your computer. Notice the "Push" option in the toolbar. It has a "1" on it indicating that you have one revision that hasn't been pushed to GitHub.com.

Click the "Push" option. You will get a confirmation popup with some options. Make sure that "Push to repository" has "origin" selected and the checkbox next to "master" is checked. Then click "OK". Once SourceTree is finished, the "1" will no longer be on the "Push" option.

Those are the several of the most basic Git functions that you will use in SourceTree.

[Back to Lesson 4 outline](https://github.com/live-and-learn/git-learning/tree/master/lesson-4 "Back to lesson 4 outline")