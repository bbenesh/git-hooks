# git-hooks
My global git hooks -- most notably, they play audio files when you pull, commit, and push.

1. git clone git@github.com:zombree/git-hooks.git .git
OR download to your computer, save in your home directory, and make sure to name the top-level directory .git. If you don't want this to live in your ~/.git, you need to go into all the hooks that don't end in .sample and update the paths in them.

2. documentation on how to install these globally...

I put these directly in my home directory and configure them as global so that they run in every project on my computer.
To make these work globally, run:
git config --global core.hooksPath path/to/wherever/you/cloned/this/directory

These will now run in any new git repo you create on your local computer. In order to get them to run on any projects that already exist on your local, cd into that project and run `git init` to re-initialize the project. This won't harm anything, it will just refresh your git so that it is aware of the new global config you just created.

3. with info on how to install them on just a local project.

You could also just take the /hooks and /sounds directories and place them in the .git directory of one specific project, and then they would run just for that project. Make sure you run `git init` in your local project after you add these new hooks.


Resources: a list of all the urls I hit up when piecing together how to accomplish this

http://stackoverflow.com/questions/17219540/how-can-i-play-a-sound-whenever-i-commit-to-git
https://collectiveidea.com/blog/archives/2010/08/03/happy-git-commits
#outdated http://stackoverflow.com/questions/2293498/git-commit-hooks-global-settings
http://stackoverflow.com/questions/1977610/change-default-git-hooks/37293001#37293001
https://github.com/git/git/blob/6675f501f6b987dbdb0dbeb1d2efeb5a27fc41a7/Documentation/githooks.txt
https://www.atlassian.com/git/tutorials/git-hooks
http://stackoverflow.com/questions/5084100/post-commit-hook-not-running
https://git-scm.com/book/gr/v2/Customizing-Git-Git-Hooks
