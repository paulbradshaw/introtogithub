# How to export a project from CodePen and publish as a webpage on GitHub Pages

[CodePen](http://codepen.io/) is a website that makes it easy to edit code and preview the results. Below are a couple of other tutorials which you may find useful before doing this one, as they outline how to use CodePen and one particular project using CodePen. This tutorial assumes you've played with code in CodePen and now want to publish that on GitHub Pages.

* [3 things you need to know about CodePen before using it to learn JavaScript](https://docs.google.com/document/d/1EV_VxgCCH_czuaYoretoy_gUaO9pP4BwcSpiRRANbZQ/pub)
* [Using JavaScript to pull data from the police crime API (or any other API)](https://docs.google.com/document/d/1Ao_EJbK9Yo-UPlH5JBNohvxVn7ll76ENzkw4QH0W0gk/pub)

If you don't have a project to export, you can always [fork this one](http://codepen.io/paulbradshaw/pen/JWzPmO) and go from there.

## Exporting the project from CodePen

Once your CodePen project is ready to be published, you have a number of options:

* The **Full Page View**: this removes the 3 code editing windows and just shows your webpage, with a bar across the top showing the title of the Pen and the CodePen logo. You can access Full Page View by clicking on *Change View* in the upper right corner, and selecting *Full Page View*. You'll notice the URL is the same as before, but with `pen` replace by `full` like so: `http://codepen.io/paulbradshaw/full/JWzPmO/`
* The **Embed** option: this is in the lower right corner and opens a window where you can find code to use to embed your pen on another website. 
  * The top area of this window allows you to specify the *Theme* (choose *Light* to make the header bar less intrusive), *Default State* and *Editable State*. 
  * The middle area shows a **Preview** of how the embed will look. Note where it says *Toggle tabs below to affect what shows by default*. Normally, the embed shows a split screen between code and result - but you can change this. Toggle the *HTML* button off (so that it is pale grey), and toggle the *JS* button off, but leave the *Result* button toggled on (dark grey) and you can just embed the result.
  * The bottom area shows the resulting code that you can copy and paste into a webpage to embed it. There are 3 options here: WordPress shortcode (if you're embedding on a WordPress.com site); iframe; or HTML. Choose HTML in most cases.
* The third way to publish your CodePen project is to *Export* it. The button for this is also in the lower right corner. This is what we're going to do in this tutorial. Click on that, and then select *Export .zip*

![](https://raw.githubusercontent.com/paulbradshaw/introtogithub/master/images/export_codepen.png)
