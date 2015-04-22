Something you should know about SourceTree is that it only manages repositories. It does not include a file editor so you will use other applications to edit files. SourceTree does show you what has changed in the revisions in the commit history and its display of this information works well for me. However, you can set up SourceTree to use a separate application to show file differences.

When you start SourceTree for the first time it will appear with the Repository Browser window. This is a small window that you use to add the repositories that you plan to manage in SourceTree. You can organize repositories in groups that look like folders in this window. In my Repository Browser, I have several groups that I have collapsed so that just the group names are showing.

When you want to manage a repository you just click on it and the repository window appears for that repository. If you want to see the Repository Browser window again press Cmd+B or choose "Show Repository Browser" from the Window menu.

To clone your fork of the sample repository for this course:
1. Open the repository browser if it is not showing.
2. Click on "New Repository" and choose "Clone from URL"
3. Complete the requested information. The "Source URL" is the URL you copied from the repository page of your fork of the course sample repository. The other two fields are where you want the repository to be on your computer and the name you want it to have in the repository browser screen. You should have the name be the same as the actual repository name in GitHub.com (git-learning in this case).
4. Once you enter the requested information and click "Clone", SourceTree will show the progress of the cloning and then open a repository screen for that repository. The repository screen has a toolbar of Git commands at the top, the revision or commit history below the toolbar, commit detail for the selected commit in the commit history, and branch information on the left sidebar.

In the next video, we will make changes to existing files in this repository.

[Back to Lesson 4 outline](https://github.com/live-and-learn/git-learning/tree/master/lesson-4 "Back to lesson 4 outline")