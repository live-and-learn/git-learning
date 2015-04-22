SourceTree periodically checks the remote copy of the repository on GitHub.com for any changes. If someone else has pushed changes to the repository on GitHub.com, the "Pull" option on the toolbar will get a red number indicating the number of revisions in the remote repository that you don't have.

Those revisions will show up in the commit history list, but the bolded, or current, revision will be the one before any new revisions that have not been pulled.

There are two ways to get the latest revisions, but for this course we will use the "Pull" option on the toolbar. Click the "Pull" option. Make sure that "Pull from repository" has "origin" selected and "Remote branch to pull" has the "master" option selected. Also, make sure that "Commit merged changes immediately" and "Rebase instead of merge..." are both selected. Not selecting these may result in duplicating the commit history for the repository.

After you click "OK" you will no longer see the red number on the "Pull" option on the toolbar and the latest revision will now be in bold. This indicates that the changes up to and including that revision are those that you would see if you looked at the file contents on your computer.

To keep current with the changes in a repository, and avoid headaches with file conflicts, get in the habit of checking for and pulling remote changes often.

With your fork of the repository for this course you won't likely see changes to its files unless you make them. However, when working on a shared repository with a team of other developers, changes to the remote repository will be common.

With that much instruction, you are now ready to do a typical workflow on a GitHub.com repository using SourceTree.

[Back to Lesson 4 outline](https://github.com/live-and-learn/git-learning/tree/master/lesson-4 "Back to lesson 4 outline")