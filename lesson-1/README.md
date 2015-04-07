Welcome to code version control using Git, GitHub.com, and SourceTree.

[Click here to watch a video](http://live-and-learn.github.io/assets/git-learning/lesson-1-version-control-using-git-github-and-sourcetree.mp4 "Video about version control and Git") introducing file version control and Git.

START: lesson 1 video transcript
Version control isn't anything new. You've probably already been using it whether you're actually using a version control system or just doing it manually. As you work on a computer you may do things like adding dates to filenames to keep track of what version of the file this may be. Some examples of keeping revisions of a file this way are index-3-20.html or index_old.html. You may want to have different versions of your file and may have one has some material in it that you needed to take out before you submitted the file. When you have more than one person working on a file, you will run into problems if you don't have a good way to manage versioning and, if you're working on source code, this is especially going to be a problem.

Over the years there's been lots of systems or programs that have been written to make version control better and easier. A fairly new and popular versioning system is called Git.

Git has several benefits. Git is fairly easy to understand. It results in distributed repositories (a repository is a place where your files live in a Git versioning environment). A Git repository can be on your computer, it can be on someone else's computer, and it can be on GitHub.com. That's what is meant by a distributed repositories. This promotes having several backups of the files. Other advantages are that it's easy to control who has access to a Git repository, easy branching of code (well, easy enough compared to other systems), Git is fast and requires very little space for versions of files, and it has automatic end-of-line conversion (not really something to worry about, but it is an advantage).

Let's talk about some of the Git commands and a typical workflow where you would use them. This part won't have enough detail to use the commands. The idea here is to just get you familiar with the names of the commands.

The basics of version control is getting a copy of the repository or the code, making changes to the files, testing the changes, saving them to a revision, and making them available to others working on or using the same code. There is also being able to branch the code and merge in branches. These repository and version operations have Git commands to do them.

To use any Git command you first type "git" so your computer knows what app the command is associated with. Lesson 3 will have more about this, but for now, just know that you will prefix every Git command with "git ".

The first Git command you are likely to use is the "clone" command. This is how you get a copy of the code or repository of code that you're going to work on.

Once you have a copy of the repository of files, you make changes to the files using whatever editor you use. To add a new file to the repository revisions, you first have to tell Git that you want to start tracking the file. You do this with the "add" command. Once you've done that, you commit the new and changed files with the Git "commit". It's with this command that you type a message that will be stored with the revision to summarize what the!?? changes were about. Git will provide exact details of the changes themselves.

By the way, if you want to find out if you have changes to commit, you can use the Git "status" command.

When you commit changes, you're actually committing them to your local copy of the repository and their revision information actually still lives on your local box. To copy your revision to the original repository you use the Git "push" command.

If you want to make a local copy, or branch, of your local Git repository so that you can work on a feature that might take a while to complete or that is an experiment, you can tell Git to make a branch. To do this you use the Git "branch" command. Creating and using branches also involves another Git command called "checkout". To merge a branch back to the main or "master" branch of the repository, you use the Git "merge" command.

To create a new repository, you use the Git "init" command and then add files and commit the revision.

Now a typical workflow using Git would be something like this:
You clone a repository to get a copy on your computer. If this is a computer application or web site, you then install the dependencies so you can run it on your computer. Then you make changes to the files and test the changes on your computer. If there are automated tests for the code, you should run them. It is recommended that you have someone else review your changes as a safety check. Then you commit the changes which creates a revision in your local Git repository and then push the changes to the remote repository. Then you should test the changes on actual web site to make sure that they are working there. Then you repeat this process except that, instead of using the clone command again, you will now use the Git "pull" to get any revisions that others have made. (When you do that there is an important concept called "rebasing" that we will explain later.)

Now these are not all of the Git commands, but they are very common ones that will get you off to a good start.
END: lesson 1 video transcript
