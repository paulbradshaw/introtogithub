# Notes on GitHub

## Stage 1: Getting to know the GitHub website

GitHub allows you to share files and create webpages, but it also allows you to copy and adapt ('fork') code made by others, and collaborate with others. You can edit, upload and delete files on the website, although below I've outlined other things you can do beyond the website too.

Things to do once you've set up an account on GitHub:

* Create a repository (a 'repo') and tick the box that automatically creates a README.md file
* Open that README.md file on GitHub, and then click the edit button
* Read about Markdown and edit your README.md file (the .md means markdown) to practise basic Markdown
* Create a new file in your repository, with a .md extension

## Stage 2: Getting to know the GitHub desktop client

Install the GitHub 'client' on your computer. This can be used to edit files locally, but also to add new files and folders to your repo and upload ('sync') them with your account on GitHub. If you've ever used a service like Dropbox you'll have done something similar: edited and moved files locally, with changes reflected on the online version that can be accessed from anywhere.

* Clone a repo from GitHub to your local client
* Open that repo's files locally, on your computer
* Edit those files
* 'Commit' your changes with a comment (this just means GitHub notes the changes)
* 'Sync' your local changes (this means they are uploaded to the GitHub repo online)

## Stage 3: Creating a branch in your repo

Branches allow you to create different versions of a project, in order to experiment with different ideas without affecting the original. It also allows other people to collaborate with you and create versions too. If you want to merge your 'improvements' with the original, you can submit a 'pull request' to make this happen.

Clone a repo to your GitHub client. Open it, and click on the 'branch' button along the top (to the left of the button/dropdown saying 'master')

* Give your branch a new name. Now you will have two copies of anything you created in the repo: the original 'master' set of files; and a new 'branch' of those. Once you create the branch, that branch is automatically selected, and any changes you make will *only affect that branch*. But you can switch between branches by using the dropdown button next to the 'create branch' button you just used.
* Open the repo's files locally, and edit something about them. These files are within the *branch* of the original, which are a copy - so it does *not* affect
* Commit changes as you go.
* Once you want to upload it, sync with GitHub
* On your repo on GitHub.com you should now see the new branch - and you should also see the option to **Compare & pull request**. Clicking that button begins the process of merging any changes back into the 'master' version of your project.
* So click it. It will tell you that it is *able to merge* and if you scroll down you can see the differences between the two versions (highlighted in green, with the changed lines highlighted in red)
* If you're happy, click **Create pull request**
* Now you're told *This branch has no conflicts with the base branch*. Click **Merge pull request**, and **Confirm**
* Your master version is now the same as the branch you created. You can confirm this back on the main page of your repo.

## Stage 4: Managing conflicts in a branch

Sometimes when more than one person is working on a project, their changes *conflict*. Here's what happens.

* Make a change to a file in your repo on your computer. Commit it, but *don't sync yet*
* Make a change to the same file on GitHub.com in the same branch. Commit it.
* Now, on the GitHub client on your computer, try to sync your changes from your branch.
* The GitHub client will raise an error - telling you that there were conflicting changes and offering you the option to show the conflicting file, or to open it in an editor. Open the file.
* Where conflicts exist in the file you should see a `=======` with one version above, and one version below. Above and below each version you will see `<<<<<<<` or `>>>>>>>` followed by an indication of which version it came from. Edit it so you have a version you're happy with.
* Make sure you commit again, and sync again.


## Stage 5: Managing conflicts in a pull request

* In a branch other than 'master', make a change to a file in your repo on your computer. Commit it, but *don't sync yet*
* Make a similar change (but not the same) to the same file on GitHub.com on the 'master' branch. Commit it.
* Now, on the GitHub client on your computer, sync your changes from your branch.
* The conflict is not raised until you try to merge the two versions.
* Click on the 'Pull requests' tab
* Click 'New pull request'
* You need to select the two branches being merged. For *base:* choose 'master' and for *compare:* choose your other branch. Click **View pull request**
* Click **Resolve conflicts**
* You will see a similar view to that detailed above, with conflicts highlighted in red. Edit the conflicts to specify what you want the new version to be like.
* Mark as resolved
* Commit changes
* Merge pull request
* Confirm merge

## Stage 6: Forking others' code

You can fork someone else's repo, and then submit a pull request to have it reintegrated into the main version.
