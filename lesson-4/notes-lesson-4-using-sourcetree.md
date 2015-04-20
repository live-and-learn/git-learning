Before actually using SourceTree. Let's talk about some similarities and difference between using Git at the command line and using an app like SourceTree. When you use SourceTree it is issuing the Git commands for you. Buttons are usually labelled with the name of the Git command they perform.

Both Git commands and SourceTree can act on the same repository (you can manipulate the same repository with Git commands and SourceTree). SourceTree does not make its own version of the Git repository. You may want to perform Git commands from the command line or from SourceTree depending on which is more convenient at the moment. You can do that.

Some differences are that SourceTree has a visual interface that may make some operations easier, however, Git commands may be faster to do because no mouse movement is required.

Check for understanding:
Name two similarities and two differences between using Git terminal commands and a Git client app like SourceTree.
Similarities:
1.
2.

Differences
1.
2.

Check for understanding:
Name two similarities and two differences between using Git terminal commands and a Git client app like SourceTree.
Similarities:
1. Both use Git commands.
2. Both can act on the same repository (you can manipulate the same repository with Git commands and SourceTree).

Differences
1. SourceTree has a visual interface that may make some operations easier.
2. Git commands may be faster because no mouse movement is required.


Ok. Let's start using SourceTree. Download SourceTree from http://www.sourcetreeapp.com/ and install it.

SourceTree has two screens that you will use the most. The repository browser screen lists any repositories that you have told SourceTree about. You can show this screen by pressing Cmd + B (Mac) or selecting "Show Repository Browser" from the Window menu.
The other screen is the repository screen which is the screen you will use to manage a repository.

To clone your fork of the sample repository for this course:
1. Open the repository browser
2. Click on "New Repository" and choose "Clone from URL"
3. Complete the requested information. The "Source URL" is the URL you copied from the repository page of your fork of the course sample repository. The other two fields are where you want the repository to be on your computer and the name you want it to have in the repository browser screen. You should have the name be the same as the actual repository name in GitHub.com (Git6350Tutorial in this case).
4. Once you enter the requested information and click "Clone", SourceTree will show the progress of the cloning and then open a repository screen for that repository. The repository screen has a toolbar of Git commands at the top, the revision or commit history below the toolbar, commit detail for the selected commit in the commit history, and branch information on the left sidebar.

Now add some files to that repository folder and make some changes to existing files. Then go back to SourceTree with the "Git6350Tutorial" repository screen showing. The commit history has the most recent item at the top and above that is an entry labelled "Uncommitted changes". Select that and you will get detail showing the file or files you have changed or added.

Below the commit history section of the screen you will see the names of these files. Changed files will have a yellowish orb next to them and new files will have a question mark icon next to them. When you click on a filename you will see detail showing the changes to changed files and the entire file for new files.

Notice the checkboxes to the left of the filenames. Checking the boxes indicates that you want to perform some action on the files. Usually new files are not automatically checked and changed files are. For now, make sure all of the boxes are checked. Up to this point you have already used the Git "status" command because SourceTree shows you the new and changed files.

Now click "Commit" option in the toolbar. At the bottom of the screen you will now see an area where you can type the message for the commit. Remember that the first line should be 50 characters or less and should be considered the subject of this revision. SourceTree does not impose any limits on the text, but when the message shows up in GitHub.com the 1st line will be truncated and put in a subject-like field with the remainder of that line and the other lines in another text box.

Type your commit, or revision, message and click commit. The first time you select new files and click "Commit", SourceTree will ask you to confirm the addition of new files. If you do not want to be asked again, check the checkbox, and then click "OK". Otherwise, just click "OK".

At this point you have just used the Git "add" and "commit" commands. Now you will notice that the "Uncommitted changes" phrase has been replaced with the revision represented by part of your commit message.

Remember that at this point the changes are still just on your computer. Notice the "Push" option in the toolbar. It has a "1" on it indicating that you have one revision that hasn't been pushed to GitHub.com.




Click the "Push" option. You will get a confirmation popup with some options. Make sure that "Push to repository" has "origin" selected and the checkbox next to "master" is checked. Then click "OK". Once SourceTree is finished, the "1" will no longer be on the "Push" option.

Those are the most basic Git functions that you will use in SourceTree. SourceTree periodically checks the remote copy of the repository on GitHub.com for any changes. If someone else has pushed changes to the repository on GitHub.com, the "Pull" option on the toolbar will get a red number for the number of revisions in the remote repository that you don't have.



Those revisions will show up in the commit history list, but the bolded, or current, revision will be the one before any new revisions that have not been pulled.

There are two ways to get the latest revisions, but for this course we will use the "Pull" option on the toolbar. Click the "Pull" option. Make sure that "Pull from repository" has "origin" selected and "Remote branch to pull" has the "master" option selected. Also, make sure that "Commit merged changes immediately" and "Rebase instead of merge..." are both selected. Not selecting these may result in duplicating the commit history for the repository.

After you click "OK" you will no longer see the red number on the "Pull" option on the toolbar and the latest revision will now be in bold. This indicates that the changes up to and including that revision are those that you would see if you looked at the file contents on your computer.

With that much instruction, you are now ready to do a typical workflow on a GitHub.com repository using SourceTree.

Here are a few more Git commands that are easy enough to use in SourceTree.
To make a branch using SourceTree use the "Branch" option in the toolbar. You don't have to make the branch before making changes to files. If you have already made some changes to files and decide to make a branch with those changes, just click the "Branch" option, enter a name for the branch, and click "Create Branch". The branch will be created (its name will show up in the "BRANCHES" list in the left sidebar) and will become the current branch as indicated by its name in bold type. (If you want to change back to the "master" branch just double click on the branch name "master". That executes the Git "checkout" command.)


Then make changes, commit then, and push the branch to the remote repository if you want to. Once you are finished working on the branch, switch to the "master" branch (double click it) and then right click on the branch you created and choose "Merge <name of branch> into master". A "Confirm Merge" popup will appear. Make sure that the option to "Commit merged changes immediately" is checked and click "OK".



Once the branch has been merged in the "master" branch, it will not be automatically deleted. To delete the branch, right click on the branch name and choose "Delete <name of branch>". A "Confirm Branch Deletion" popup will appear. Click "OK".

Now let's talk about pull requests. For these lessons, you have been make changes to the fork you created from the sample repository for this course. If you wanted to request that the revisions you made to your fork get pulled into the original repository, you can create a pull request.

Pull requests are not just for when you don't have write access to a repository. For example, you could be working on files in a repository along with other people and all of you have write access to the repository. However, you want to commit some changes, but you want someone else to review them and no one is available at the moment. You can create a branch with your changes, commit you changes to that branch, push branch with the changes to GitHub.com. Then create a pull request.

Go ahead and create a pull request for the original sample course repository with the revisions you have in your fork. To do this, choose "Create Pull Request" from the "Repository" menu.

Make sure your options look like this and click “Create Pull Request On Web”.


You will be directed to an "Open a pull request" page on GitHub.com. Type a title for the request, a short description if you want to, and click "Create pull request". The owners of the original repository will be notified of the request. Don't worry that the request will cause any problems. Someone with write access to the original repository would have to merge the pull request to add your changes to the original repostiory.

Ok. One last command and it is the Git command that is used to get a repository started. However, when working on existing projects or with other developers, you are not likely to use it very often.

To create a new repository using SourceTree, go to the "Repository Browser" screen, click "New Repository" and choose "Create local repository". Then complete the information for where you want it to be and what you want to call it. You also have the option to create the remote repository on GitHub.com at the same time. Click "Create".
