# Creating webpages and websites on GitHub

You can use GitHub to create webpages or whole websites. There are a couple of main ways to do this:

* Use the automatic webpage generator to take your existing Markdown files and turn them into webpages
* Create HTML files yourself

[You can find more information here](https://help.github.com/categories/github-pages-basics/)

## Choosing a repo to publish from

There are 3 main places you can publish your website from:

* The `master` branch of your project (which is created when you set up your repo)
* A folder called `/docs` in that repo
* Or a *branch* you have called `gh-pages`

[This guide](https://help.github.com/articles/configuring-a-publishing-source-for-github-pages/) explains how to set up GitHub pages to publish your site from different branches or folders in your repo. Below I will explain the process step by step.

### Option 1: creating a /docs folder

If you want all your website files to live inside a folder called 'docs', you need to create that. But there's no button to 'create folder'!

Instead you need to click '**Create new file**'. Then, when naming the new file, type `docs/index.html`

This will create a folder called `docs`, *and* within that your new file called `index.html`. 

Save it (by clicking Commit changes) and both the folder and file are created. You can come back and edit `index.html` later.

### Option 2: creating a gh-pages branch

Typically a branch is a way of working on a different version of a project: when you create a branch of a repo in GitHub it automatically copies all the files from the original 'master' branch. However, in this case that's not really the reason: a `gh-pages` branch (it means GitHub Pages) is just a place to put all your website files, away from the main repo.

To create a new branch click on the button that says *Branch: **master***, just above the list of the files in your repo.

This opens up a drop-down menu with a text box that allows you to *Find or create a branch...*. Type `gh-pages` in that box and underneath you will see an option to **Create branch: gh-pages**. Click that.

At first it will look like nothing has happened. But look closer: *now* the button just above the list of files should say *Branch: **gh-pages***.

This is the new branch you just created. Because it copies all the files from your master branch, it will look exactly the same - but trust me: you're now in the branch that will be used to create your website.

Create a new file in this branch called `index.html`. You don't need to add anything to it yet, but this will be the homepage for your GitHub Pages site. It might also help if you delete any other files that were copied across from the master branch but that you won't be needing in the website.

### Option 3: use the master branch

This might appear to be the easiest option (no need to create new folders or branches) but actually it's going to cause the most confusion in the long run, as you'll be storing both your website and repo in the same place.

If you do want to use the master branch, though, there's only one thing you need to do: create a new file called `index.html`. If you don't do this, then GitHub will use your readme.md file as the basis for the homepage on your site. Now, to edit that index page.

## Activating your GitHub Pages website

Once you've chosen whether to put your website in `/docs`, the `gh-pages` branch, or the `master` branch, you're ready to activate the site. 

To do this, click on **Settings** in the upper right corner, or just add `/settings` to the end of the repo URL.

In the settings page scroll down to the **GitHub Pages** section. The first part, **Source**, has a drop-down menu where you can tell GitHub to begin publishing a website based on this repo. Click on this drop-down and select the option you want (if you haven't created the folder or branch needed, that option will be greyed out until you do).

GitHub will now begin publishing your website. Above you should see an area where it tells you the URL of the new site - it will be your username, followed by github.io, followed by a slash and the repo name. My username is `paulbradshaw`, for example, so all my GitHub pages sites start with `paulbradshaw.github.io/`, followed by the repo name. The URL for the GitHub Pages site for the repo `introtogithub`, then, is `https://paulbradshaw.github.io/introtogithub/`.

It will take a few seconds to create your new site, but after a while when you click on your GitHub Pages link, you should be taken to the working webpage (which may be blank for now). 

## Editing your homepage

The homepage of any website will always have one of just a few names: `index`, `default` or `home` followed by `.html` or `htm` are typical examples. When a browser goes to a URL like `https://paulbradshaw.github.io/introtogithub/` the server [will look for a file with one of those names](https://uk.godaddy.com/help/what-file-displays-when-someone-browses-to-my-domain-name-60). For example the URL `https://paulbradshaw.github.io/introtogithub/` will show you the same thing as `https://paulbradshaw.github.io/introtogithub/index.html`

All you really need to know is: *make sure you call your homepage file* `index.html`. 

Obviously you can edit that HTML document however you like, making sure to use HTML to do so.

You can then add other files with any name you like, and link to them accordingly.

Each time you save changes, you can test the results 
