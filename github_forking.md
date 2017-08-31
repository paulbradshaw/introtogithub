# Forking in GitHub

Forking is very similar to cloning. The key differences are that cloning simply makes a copy; forking not only makes a copy, but creates a connection between your (forked) version of the project, and the original. You can, for example, choose to update your project with any new additions to the original; or submit your changes to be considered for inclusion in the original project (a pull request).

You can fork someone else's repo, and then submit a pull request to have it reintegrated into the main version.

## Getting started with forking

At the top of this repo is a button to '**Fork**' it. Click that button.

A copy of this repo will be created within your own GitHub account. Underneath the name you should see a link back to the original.

I've [created a file which you can edit here](https://github.com/paulbradshaw/introtogithub/blob/master/editme.md). 

Edit that file, add some more text, and then commit those changes (and sync if you're using the GitHub client rather than the website)

## Create a pull request

On your repo webapge, go to the pull requests tab and click **New pull request**. You will be shown the differences, (and hopefully "This branch has no conflicts with the base branch"). 

Click **Merge pull request**, and **Confirm**

The creator of the original repo now has to confirm your pull request for it to be reincorporated to the original version.

## Updating your version so it reflects changes to the original

It may be that you want to fork a repo not to suggest changes but just to keep updated with any changes to the original. The process for this is similar to the pull request above, but you need to switch the 'base fork' and 'head fork'.

1. On your repo webapge, go to the pull requests tab and click **New pull request**. 
2. You will be taken to the *Comparing changes* page. If you have made no changes to the repo, none will be shown, and it will say *Try switching the base for your comparison.* Click on this to switch the two bases. If that option is not available, change the 'base fork' dropdown to the name of your own fork (it will start with your username), then click *compare across forks* above to show the forks again, and finally change the 'head fork' to the original repo that you want to update from. 
3. You should now have your own fork selected in 'base fork', and the repo that you want to update from in 'head fork'. Any changes ('commits') will be shown in a list underneath. Click **Create pull request**.
4. The page will change to *Open a pull request*. You need to give this pull request a title: type 'Updating my fork from original' or something similar. This is just to help you or someone else understand the history of changes made to your repo. You can also add a description if you want.
5. Click **Create pull request** underneath the box
6. Now it should confirm that there are no conflicts with the 'base branch' (yours). Click **Merge pull request**, and **Confirm**

Your fork should now be up to date with any changes made since you forked it (or last updated it).

*Geek note: at the last stage (6) above, you can - instead of **Merge pull request**, choose **Rebase and merge**. This creates a simpler commit history. You can [find out more about rebasing here](https://www.sbf5.com/~cduan/technical/git/git-5.shtml).*

