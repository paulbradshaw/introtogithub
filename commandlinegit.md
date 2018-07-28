# Using Git on the command line

**Git** is not the same as GitHub - it is a "version control system" created in 2005. GitHub, a website hosting service for *using* Git, was founded a few years later, in 2008.

In other words, GitHub is an easy way to use Git, but not the only way. You can use Git on the command line outside of GitHub, or as part of GitHub.

You can find the book [Pro Git available online for free here](https://git-scm.com/book/en/v2). This details how to use Git on the command line. A [section of the book is dedicated to GitHub specifically](https://git-scm.com/book/en/v2/GitHub-Account-Setup-and-Configuration)

## Getting started with Git on the command line

You [can install Git](https://www.linode.com/docs/development/version-control/how-to-install-git-on-linux-mac-and-windows/) and [follow the instructions on setting it up here](https://help.github.com/articles/set-up-git/)

Once you've installed Git, you can create (initialise) a repository by navigating to the folder using command line (type `ls` to list files in the current directory and `cd` to change the current directory until you are in the one you want to initialise) and typing:

`git init`

Alternatively you can *clone* an existing GitHub repo by copying the URL, then navigating to the folder where you want to put the new repository, and typing `git clone` followed by the URL you just copied, e.g.:

`git clone https://github.com/paulbradshaw/introtogithub`

By default it will use the repo name as the folder name - in this case `introtogithub`. Make sure you move into that folder using `cd`, so in this case `cd introtogithub`

## Changing files

![](https://git-scm.com/book/en/v2/images/lifecycle.png)

The Pro Git book [has an excellent diagram](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository) showing the differences between difference file 'statuses' in Git (shown above):

* **Untracked** files are new files which have been added *or* old files which have been deleted since the last commit. When you commit, these files will need to be *staged* if you want to add or remove them.
* **Unmodified** files have not been changed since the last commit - so no updates need to be recorded
* **Modified** files have been changed and will need to be *staged* for changes to be recorded
* **Staged** files are those which are marked to be committed

If you type:

`git status`

Then you will be given information about the status of the files in the repo: which ones are untracked, or modified but not staged, and which changes are yet to be committed.

You stage new files to be added, *or* changes to existing files, by using `add` like so:

`git add NAMEOFFILE.md`

Obviously the last bit needs to be replaced with the actual name of the file, including any file extension such as `.txt`.

When you're ready to commit those changes you type:

`git commit -m "COMMIT MESSAGE HERE"`

Now that changes have been committed, they still need to be *pushed* from the local version to GitHub's remote version. The command for that is `push`, and [you need to specify where you are pushing it *from* and *to*.](https://help.github.com/articles/pushing-to-a-remote/)

Typically you are pushing it *from* the `origin` and *to* the `master` branch on GitHub. For that the full command is:

`git push origin master`

You will then be asked for your GitHub username, and then for your password. If you have two-factor authentication set up you will probably get an "authentication failed" message. To address this you will need to [create a personal access token to use as a password when authenticating to GitHub on the command line using HTTPS URLs.](https://help.github.com/articles/accessing-github-using-two-factor-authentication/#using-two-factor-authentication-with-the-command-line) - [explained here](https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line/)
