## Smart Drag and Drop Support in [LightPaper](http://lightpaper.ashokgelal.com/)

`Added in ver 1.0`

In ver 1.0, we added drag-and-drop (DnD) support in [LightPaper](http://lightpaper.ashokgelal.com/). DnD in ver 1.1 has got even better and smarter. Now, when you DnD a link or images, it actually inserts the corresponding Markdown tags for them.

One of the things that people struggle with Markdown, and that includes me, is remembering the syntax for inserting images and links. Is it `()[]` or `[]()`? [LightPaper](http://lightpaper.ashokgelal.com/) kind of already helps you with a handy shortcut -- `⌃⇧L` for adding a link and `⌃⇧I` for adding an image -- but still it is hard to remember those shortcuts.

Often times I've found myself just dragging and dropping links and then "fixing" it. Now with [LightPaper](http://lightpaper.ashokgelal.com/) 1.1 all you have to do is just select a text (or not) and drop links from your browser address bar or drop your images. What's even better is that you can select multiple texts and then drop your link(s); [LightPaper](http://lightpaper.ashokgelal.com/) takes care of inserting paths to all those selected texts and preserves the selection(s). Try selecting multiple texts -- press ⌘ and select -- and dropping a URL. Once you are done typing link title, just hit tab or enter key and you'll be taken to the end of the link so that you can continue typing.

![gif for link drag-and-drop](screenshots/links_drag_drop.gif)

### Relative Paths for Images

Ver 1.0 not only fixed issues with relative paths for images but also added a way to set any folder as a base folder - right click on a folder from the sidebar and select `Set as Base Folder`. This helps rendering your images properly if you have your images in a different folder. This is especially helpful with static site generator such as [Jekyll](http://jekyllrb.com/).

Ver 1.1 takes this to the next step - when you drag and drop images it "calculates" the paths in relative to your base folder automatically for you. This way you don't have to go and correct your paths.

![gif for image drag-and-drop](screenshots/image_drag_drop.gif)

Please try out this new feature and let me know what you think of it.

If you haven't tried [LightPaper](http://lightpaper.ashokgelal.com/) yet, go ahead and try a 7 days full feature trial.