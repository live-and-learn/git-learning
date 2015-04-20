Slide 1
Welcome to Git Basics: Version Control Using Git, GitHub.com, and SourceTree. These tutorials are designed to help you familiarize yourself with Git as a version control process, as well as with some of the tools which are available to help you use Git – including GitHub.com and the SourceTree application.

Slide 2
Git is a system for Version Control. Version control isn’t a new concept, and you are probably doing it whether you realize it or not. Version control, whether formal or informal, has two main purposes – to keep the file backed up or saved in more than one location, and to save multiple copies or show a record of changes that have been made.

Informal version control includes renaming files (for example, adding a date or a descriptor (like old, new, latest) to the file name) or saving multiple copies of a file in various locations (usb drives, hard drives, and the cloud). Informal version control works fairly well, as long as only one person has editorial abilities at any given time. Two of the bigger issues with informal version control are:
1. Combining different sections from multiple files (taking a section of code from file A and a section of code from file B and storing them both with the rest of the code for file C.
2. Concurrent work – managing multiple editors on a single file – keeping them from undoing each other’s work and keeping track of who did what.

Formal version control systems keep (and expand) the benefits of backups and revision history that exist in informal version control, but have features that make it not only possible, but often fairly simple, to manage multiple contributors and combine (or merge) their changes in the files.

Slide 3
Git is a fairly new, and extremely popular, version control system. There are several advantages to Git as a formal system for version control.
1. Git is fairly easy to understand – most people can pick it up fairly quickly.
2. Normal use of the Git system creates a ‘distributed repository’ – meaning that active files have multiple backup copies.
3. It is easy to control access to a Git repository (like a shared file folder)
4. Compared to other version control systems, Git makes branching code fairly easy. Branching code allows you to test new features without disrupting live code.
5. Finally, Git is fast and requires very little space for storing files on a local machine.

Slide 4
The basic workflow for using any version control system is:
1. Start by getting an updated copy of the code you will be working on. As a part of this step, make sure that you have any other necessary files or software to enable you to test the code.
2. Sometimes, especially when you are making large changes or adding new features, it is best to create branches of the code so that you can have multiple working versions of the code at the same time.
3. Make changes and test them on your local machine.
4. Review your changes with a coworker. This has proved helpful to catch problems and improve code.
5. Commit the changes to your local Git repository. If you did make a branch of the code, this step will involve merging that branch into the main or ‘master’ branch.
6. Upload or push the changed code to the shared repository (GitHub.com in this case) so that it is available for other developers or users.
Please note, in most of our examples and throughout the tutorial, we will talk about using Git (and related tools) to store, share, and work on computer code. This is a major use of version control systems. However, you can also use Git to store, share, and work on presentations, papers, or anything else.

Slide 5
The git “init” command is used to create a new repository on the local machine, rather than creating the repository through GitHub.com or using an existing repository. It is less commonly used than the other commands we will be discussing in this course.

The first Git command you are likely to use is the "clone" command. This is how you get a copy of the code or repository of code that you're going to work on.

If you want to make a local copy, or branch, of your local Git repository so that you can work on a feature that might take a while to complete or that is an experiment, you can tell Git to make a branch. To do this you use the Git "branch" command. Creating and using branches also involves another Git command called "checkout".  Now you are ready to open up the code in an editor, or even use the vim editor in the terminal, to make and test changes.

To find out if you have changes to commit, you can use the Git "status" command.
At this point it is helpful to review these changes with a coworker or supervisor.
Once you've done that, you commit the new and changed files with the Git "commit". To merge a branch back to the main or "master" branch of the repository, you use the Git "merge" command.

To add a new file to the repository revisions, you first have to tell Git that you want to start tracking the file. You do this with the "add" command.

When you commit changes, you're actually committing them to your local copy of the repository and their revision information actually still lives on your local box. To copy your revision to the original repository you use the Git "push" command.
