# Reverting to previous versions

One of the main features of GitHub is its ability to keep a record of all the changes you have made to a repo.

Every time you make a change it is called a '**commit**'.

On the GitHub website, you need to 'commit changes' every time you edit a file and want to save those changes, but on the GitHub Desktop client you can edit multiple files locally, and those then 'commit to Master'.

In both cases your commit is accompanied by a short **summary**, and you can also add a longer **description**.

## Finding the history

On the GitHub website, you can find the history of commits by going to the main repo page and clicking on the *Commits* button, or just adding `/commits` to the end of the URL. The address will look something like this: `https://github.com/paulbradshaw/introtogithub/commits`

The commit history of specific *branches* have the branch name after `commits/`, like so: `https://github.com/paulbradshaw/introtogithub/commits/reverting`

## Reverting in GitHub Desktop client

Reverting means to reverse what was done in a particular commit. So if you want to 'revert' to an earlier version, you must revert each commit that was made in the meantime.

You can revert relatively easily in the desktop client. On the left hand side you should see two tabs: *Changes*, and *History*. Switch to *History* and you can see a list of all the commits made in that repo.

To revert a commit, right-click on it, and select **Revert this commit**.

## Reverting using command line

Most reverting needs to be done on the command line. You can [find more details on how to undo various things in GitHub using command line here](https://github.com/blog/2019-how-to-undo-almost-anything-with-git). You will need to navigate to your repo folder using `ls` (to list folders in the current directory) `cd` (to change the current directory to one of those). The command `git reset HEAD~` can be used to roll back (undo) to the last commit.
