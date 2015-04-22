--Clone video
To use any Git command you first type "git" so your computer knows what app the command is associated with.

For the "clone" command, you type "git clone" and the URL or address of the Git repository. That results in a copy of that repository being made in the computer folder where you typed that command.


--Add file video
If you add a new file you first have to tell Git that you want to start tracking the file. To do this you type "git add" and the name or location of the new files.

Then you make changes to the code using whatever editor you use. And now you want to copy those changes back to the original repository. By the way, if you want to find out if you have changes to commit, you can use the "git status" command.

If you do not include the commit message (for example, "git commit *.*), you will be taken to a text editor where you can type the message.

With Git, it is good practice to consider the first line of a commit message as the subject of the commit and limit the length of that line to 50 characters. The other lines can be whatever length is needed.

In the terminal editor, you will likely have to press "i", as in "insert", first to start typing a message. When you have finished typing your message in the editor, press Esc. then type ":wq" and press Enter to save the message and exit the editor.

Once you have committed changes you're actually committing them to your local copy of the repository and their revision information actually still lives on your local box. To now make a copy of that revision or revisions you now need to push those changes using "git push" and then that copies those changes to the original repository.

[Back to Lesson 3 outline](https://github.com/live-and-learn/git-learning/tree/master/lesson-3 "Back to lesson 3 outline")