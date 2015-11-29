## What's new in LightPaper version 1.1?

#### FEATURES

* **Real Preview** - See how your post would look like on a website when you publish it ... without actually publishing it. [Learn more...](https://github.com/42Squares/LightPaper/blob/master/RealPreview.md)
* **Favorites** - Favorite a file or a folder and have it always accessible from the sidebar
* **Smart Drag and Drop Support** - Just drag and drop your images or a link, and LightPaper will add the correct markdown for you. [Learn more...](https://github.com/42Squares/LightPaper/blob/master/doc/DragNDrop.md)
* **Individual Styles** - Give each document and its corresponding preview a style of its own. Access it from `Styles` menu
* **What's new** - Know the latest and greatest features & improvements we have made in [LightPaper](http://lightpaper.ashokgelal.com) from with in the app. Access it from `Help>What is New in this Version?` menu item

#### IMPROVEMENTS
* Editor has got a lots of cool new improvements - smarter auto pairing of braces and quotes, use spaces for tabs, duplicate line(s), move line(s) up or down etc
* HTML comments within markdown are now parsed as comments in the output
* Jekyll table output is now supported in MultiMarkdown mode as well
* About 30% of the code has been rewritten using the latest Swift programming language. This makes us very happy :)
* Word counting algorithm as been optimized and is only calculated when needed
* Improves memory and CPU consumption

#### BUG FIXES

* Fixes a bug where it would crash for some users while using GitHub Flavored Markdown
* Fixes a bug where the Jekyll table wouldn't be hidden
* Fixes auto-bulleting for triple dashes (---)
* Fixes some more memory leaks