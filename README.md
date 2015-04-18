# shakespeare-git-practice
Training area for those new to git.  Fork it and clone from your own fork.

Text based on Project Gutenberg's plain text version of Romeo and Juliet by William Shakespeare.


Getting Started
======================================

Make sure you are working from a Fork of the git repository.

This means you already have a github account, and you pressed the "Fork" button
while viewing https://github.com/jennybrown8/shakespeare-git-practice on the web.

Then you went to your forked copy, so the web address changed to something like:
https://github.com/your.name/shakespeare-git-practice

Then in the lower right of the web page, look for the "clone url" piece.
As long as you remember your username and password, you can use the http url.

Copy the url to the clipboard.  Then on your own computer, bring up
the git bash command line, or your choice of graphical git client.

Run the command:

  `git clone thatUrl`

This gives you a copy of the files to get started.


Type in:

   `cd shakespeare-git-practice`

   `git status`

to see that you have no local changes yet.  You should get:

    `# On branch master`

    `nothing to commit (working directory clean)`



Instructions for Work
======================================
Each scene directory has a list of files which are pieces of
that scene, but they're not in any good order.  This is similar
to the results of putting a book through a scanner one page at
a time.  Your job is to put them back together correctly as one file.

Create a new file in each scene directory, named Scene.txt

Run `git status` to see that it has an untracked file.
Type:

   `git add scene1/Scene.txt`

   `git add scene2/Scene.txt`

   `git add scene3/Scene.txt`

   `git status`

This has added the new file to the git staging area.  You 
can commit these empty files as a starting point, and write
a message explaining what you did.

   `git commit -m "Empty placeholders for scenes"`

   `git status`

Now you're ready to start copying and pasting in the scene contents
for scene 1.

Do a small amount of work, and then git commit your changes.

   `git diff`

   `git add .`

   `git status`

   `git commit -m "Added the third section of the scene"`



Then do a small amount of work, and git commit the next set of changes.

   `git add .`

   `git status`

   `git commit -m "Added the fourth section of the scene"`

When you finish the scene, git commit and git push.

   `git add .`

   `git status`

   `git commit -m "Finished the scene"`

   `git push`

If you are working with a partner, divide the scenes between you,
and you should both push at the end of your scenes.  Note that you'll
need to git pull to bring down a copy of your partner's changes, before
you can push your own.

   `git status`

   `git pull`

   `git status`

   `git push`

Make sure you trade back and forth several times, as well as work
simultaneously several times, when working with a partner.

You can also work solo, although you won't see as interesting of
interactions with multiple commits.

These instructions are just a starting point.  You can try out 
changes of your own as well.

What happens if you rename the Scene.txt file to something
different, like FullScene.txt?  Remember to `git add FullScene.txt`
before you commit.

What happens if both of you change the same line of the same
scene file at the same time (and make it say different things), 
and you both try to commit and push your changes?  This will
cause a merge conflict.  You'll need to modify the file one
more time, then follow the on-screen instructions to finish
the commit process.

How can you view your commit history?  Try out the following.

   `git log -2`

   `git log`

   `git show d091ce`

You should also explore branching and merging, once you
understand the basics of the commit history and pushing/pulling.

