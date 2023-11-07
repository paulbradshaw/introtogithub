# Creating webpages and websites on GitHub

You can use GitHub to create webpages or whole websites. There are a couple of main ways to do this:

* Use the automatic webpage generator to take your existing Markdown files and turn them into webpages
* Create HTML files yourself

[You can find more information here](https://docs.github.com/en/pages/quickstart)

## Choosing a repo to publish from

There are 3 main places you can publish your website from:

* The `main` branch of your project (which is created when you set up your repo)
* A folder called `/docs` in that repo (or another folder you have created)
* Or a *branch* you have created (often this is called `gh-pages` but it doesn't have to be)

[This guide](https://help.github.com/articles/configuring-a-publishing-source-for-github-pages/) explains how to set up GitHub pages to publish your site from different branches or folders in your repo. Below I will explain the process step by step.

### Option 1: creating a /docs folder

If you want all your website files to live inside a folder called 'docs', you need to create that. But there's no button to 'create folder'!

Instead, back in your GitHub repo, you need to click '**Create new file**'. Then, when naming the new file, type `docs/index.html`

This will create a folder called `docs`, *and* within that your new file called `index.html`. 

Save it (by clicking Commit changes) and both the folder and file are created. You can come back and edit `index.html` later.

### Option 2: creating a gh-pages branch

Typically a branch is a way of working on a different version of a project: when you create a branch of a repo in GitHub it automatically copies all the files from the original 'master' branch. However, in this case that's not really the reason: a `gh-pages` branch (it means GitHub Pages) is just a place to put all your website files, away from the main repo.

To create a new branch click on the button that says *Branch: **master***, just above the list of the files in your repo.

This opens up a drop-down menu with a text box that allows you to *Find or create a branch...*. Type `gh-pages` in that box and underneath you will see an option to **Create branch: gh-pages**. Click that.

At first it will look like nothing has happened. But look closer: *now* the button just above the list of files should say *Branch: **gh-pages***.

This is the new branch you just created. Because it copies all the files from your master branch, it will look exactly the same - but trust me: you're now in the branch that will be used to create your website.

Create a new file in this branch called `index.html`. You don't need to add anything to it yet, but this will be the homepage for your GitHub Pages site. It might also help if you delete any other files that were copied across from the master branch but that you won't be needing in the website.

### Option 3: use the main branch

This might appear to be the easiest option (no need to create new folders or branches) but actually it's going to cause the most confusion in the long run, as you'll be storing both your website and repo in the same place.

If you do want to use the main branch, though, there's only one thing you need to do: create a new file called `index.html`. If you don't do this, then GitHub will use your readme.md file as the basis for the homepage on your site. Now, to edit that index page.

## Activating your GitHub Pages website

Once you've chosen whether to put your website in `/docs`, the `gh-pages` branch, or the `main` branch, you're ready to activate the site. 

To do this, click on **Settings** in the upper right corner, or just add `/settings` to the end of the repo URL.

In the settings page look for the **Pages** link on the left. There should be a **Branch** drop-down menu where you can tell GitHub to begin publishing a website based on the main branch of your repo, or another branch. Click on this drop-down and select the option you want.

To the right is another drop-down menu where you can select a *folder* within that branch if you want to publish files from just one folder. Or you can leave it as 'root' (which means no specific folder).

GitHub will now begin publishing your website. After a while, refresh the page. Eventually, above the area where you specified the branch etc. you should see an area where it tells you the URL of the new site - it will be your username, followed by github.io, followed by a slash and the repo name.

My username is `paulbradshaw`, for example, so all my GitHub pages sites start with `paulbradshaw.github.io/`, followed by the repo name. The URL for the GitHub Pages site for the repo `introtogithub`, then, is `https://paulbradshaw.github.io/introtogithub/`.

It will take a few seconds to create your new site, but after a while when you click on your GitHub Pages link, you should be taken to the working webpage (which may be blank for now). 

## Editing your GitHub Pages website

Now you need to remember that there are **two parts** to your GitHub Pages website:

* The website itself, which uses github.io, e.g. `https://paulbradshaw.github.io/introtogithub/`.
* The repo with the files that *generate* the website, which uses github.com, e.g. `https://github.com/paulbradshaw/introtogithub/` (more specifically, remember that those files are probably within a `gh-pages` branch, or the `/docs` folder of that repo).

To edit your website, you need to make sure that you are on GitHub.com, but then switch to the github.io website to see the results. You won't see the results immediately - it takes 5-15 seconds for the site to be updated to reflect any changes. 

For that reason you may prefer to edit the file and preview it locally (on your machine, not on the web) and then upload or paste the changes into the live version on GitHub, at least once you're comfortable with the basic process.

### Your homepage: index.html

The homepage of any website will always have one of just a few filenames: `index`, `default`, or `home` followed by `.html` or `htm` are typical examples. When a browser goes to a URL like `https://paulbradshaw.github.io/introtogithub/` the server [will look for a file with one of those names](https://uk.godaddy.com/help/what-file-displays-when-someone-browses-to-my-domain-name-60). For example the URL `https://paulbradshaw.github.io/introtogithub/` will show you the same thing as `https://paulbradshaw.github.io/introtogithub/index.html`

All you really need to know is: *make sure you call your homepage file* `index.html`. 

Obviously you can edit that HTML document however you like, making sure to use HTML to do so.

You can then add other files with any name you like, and link to them accordingly.

Test your website works by editing the `index.html` file you created earlier so it works as a basic HTML document. If you're too lazy to type it out here's a basic example to adapt:

```html
<html>
<body>
<p>This is just a demonstration.</p>
</body>
</html>
```

### Linking to other pages

With your index page created, you can now create the rest of the site. I'm obviously not going to explain web design principles here, but only how to make sure that links and images etc. work on your GitHub Pages site.

First, you can create new pages just as you created index.html - use **Create new file** and make sure that your new file ends in `.html`. 

When *linking* to those other pages, however, you need to **include the name of the repo in the link**, or just use the whole link. For example, if I add a file called `newpage.html` to this repo then the link to that should be:

`<a href="/introtogithub/newpage.html">`

Or if you just want to keep things simple:

`<a href="https://paulbradshaw.github.io/introtogithub/newpage.html">`

The same applies if you want to embed any images or media.

Once you've got to grips with the basic process that's it - you're all set to create and update your own GitHub Pages website!
