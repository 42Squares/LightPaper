## AKA Magic!

`Added in version 1.1`

[LightPaper](http://lightpaper.ashokgelal.com)'s *RealPreview* allows you to see how your post would look like on a website when publish it before actually publishing it. You just add a URL of one of your existing online posts and the class name of your post's container and you are all set.

You can add multiple sites as well and switch between them. Once the *RealPreview* is loaded you can keep typing and it gets automagically updated as well. The live preview of your real preview! Yep, Magic! :sparkles:

### Adding a site

#### Steps
1. Go to `LightPaper>Preferences>Real Preview` and click the `+` button
2. Fill up the following fields:

	*  `Article URL`: URL of one of your existing posts (required)
	*  `Name`: Name of this site - what ever you want. This just helps you to select the proper site later on (required)
	*  `Blog Type`: Select one of the provided values. If you are unsure, just select `Other` (required)

	If your site is either `Medium` or `GitHub` then the following fields are not required and hence are disabled. Otherwise at least the post class name field is required. Remember, the correctness of these fields are **very important**.
	
	*  `Post content class name or id`: The class name or the id of your container from your existing blog that hosts your content. Usually they'd be something like *post* / *entry* / *post-content* / *article-body* / *entry-content* etc If your post container has an id instead of a class name then you just add **#** as a prefix like `#content`. You can find this value by looking at the source code of your page. Browser's `Inspect Element` feature comes really handy here. 

	*  `Header class name or id`: Just like `Post content class name or id` but for the article's header.

3. Once you are done filling up all the required fields, click `Add` and you are all set to see a real preview of your document.

![RealPreview Preference](/screenshots/realPreviewPref.png)

### An example using GitHub as a sample site
Enter `https://github.com/42Squares/LightPaper` in the URL field, `42Squares` in the name field, select `GitHub` for the blog type and click `Add`.
	
This is what it would look like eventually:
![42Squares GitHub Sample](/screenshots/github_sample.png)

### Turning RealPreview on
1. Open your document and, if enabled, click the *RealPreview* button at the bottom. It looks like a R enclosed in a box.
2. If you haven't selected a site for your preview, the *RealPreview* button will be disabled. To enable it, select a preview site from `Styles>Real Preview` menu item.
3. Click on the *RealPreview* button to toggle *RealPreview* on and off. It will open an external window and shows you the simulated reality of your article.

### Providing a Title for your Article
LightPaper supports [Jekyll](http://jekyllrb.com/)'s [frontmatter](http://jekyllrb.com/docs/frontmatter/) style syntax for adding a title for your document. So to give a title, add something like this at the top of your document:

\---

title: <Your Title Goes Here>

\---

Now, if you've provided a header class or and id and [LightPaper](http://lightpaper.ashokgelal.com) can find it in the sample post, the title will be shown along with the post. There are few cases where header won't show up at all. Especially, if the site doesn't support it like GitHub for an example.

### Troubleshooting

##### `RealPreview` button is disabled
* Make sure you have added at least 1 site and have selected a default site from `Styles>Real Preview` menu item.

##### No page is displayed, I actually get a blank page
* Make sure you are connected to the Internet when you add the site.

##### The external window is open but it doesn't show the `RealPreview` just the regular preview
* Make sure you have actually enabled it by clicking the `RealPreview` button. It should be blue when it is turned on.

##### I can't see my title or my post
* Make sure you have provided the right class names or ids for your containers. Go to `LightPaper>Preferences...>Real Preview` and make sure of it.

##### I believe I did everything right but still nothing
* Ok, fire us an email. We'll try sort it out. 

##### I can see my post but not the title even though I've provided the right values
* There could be couple of reasons why this would happen. It could be that the site actually doesn't support the concept of "a title". If it does support, then it could be that your header/title container is inside the post/ article container and hence is overridden. There is not much we could do to fix this problem. If possible, you can change your blog to make sure the header/title container is outside of the post/article container.

##### I can't find my containers' class names or ids
* Please keep looking. There are millions of blogs out there and thousands of themes available for those blogs so it is very difficult for us to either categorize them or offer a one-to-one help. You can [create a ticket here in GitHub](https://github.com/42Squares/LightPaper/issues) asking for help and see if we or someone else helps you out by looking at the source of your blog and finding out those values. Please don't judge us.

##### I know how to make this feature even better
* Awesome! Please send us an email. Or even better - send us a feedback `Help>SendFeedback...` menu item

With a little bit of cleanup, this is how this document would look like if it ever got covered by [The Guardian](https://theguardian.com):
![The Guardian Sample](/screenshots/theguardian_sample.png)