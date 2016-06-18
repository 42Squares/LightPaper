### Have you tried [Real Preview](http://blog.42squares.in/2015/11/25/feature-real-preview/) and [Shadow Notes](http://blog.42squares.in/2015/12/22/shadow-notes/) features of LightPaper? No? Good Lord!

## What's new in LightPaper version 1.3?

#### FEATURES ✨

* **Multiple Folders** -  📂📂📂 Sidebar now supports multiple folders. Add as many as you want or remove the ones you don't want. LightPaper also remembers all the opened folders so you don't have to.
* **Editor Outline Navigator** - 🗺  Quickly navigate between your headers or code blocks. [Learn more...](https://www.youtube.com/watch?v=pvKF7G_E304)
    * Two-way navigation for editor outline navigator - clicking a header navigates to corresponding preview header as well.
	* Preview Outline is rewritten from scratch - looks better, gives us code monkeys 🐵 a lot of satisfaction, and supports two-way navigation as well
* 🗒LightPaper Mini: Added a preference to automatically insert shadow note's source path or URL
* 💄Added a top-level Export menu for quickly accessing exporting and copying features
    * Select markdown text and copy it as rich formatted text including images
    * Select markdown text and copy them as HTML
*  🖼 Supports different ways of setting the base URL for a document. Very useful for rendering images. [Learn more...](https://github.com/42Squares/LightPaper/blob/master/doc/Setting%20Document%20Base%20URL.md)

#### IMPROVEMENTS 💄💄💄

* LightPaper now re-renders your document when you make any changes to your sidebar's root folder(s). This makes it to render your new/modified images without having to restart LightPaper, for an example.
* 🗒LightPaper Mini:
    * Save mini documents when app gets inactive
    * `⌘+S` now continues to save a scratch or shadow note instead of persisting it to a file. You can save it to a file using `File>Save to File...` menu item or using `⌘+⌥+S` key.
    * Shadow Notes now by default selects the active tab for both Chrome and Safari.
    * Sync open notes between LightPaper and LightPaper Mini
    * Don't collapse expanded shadow notes when switching tabs or deleting a note
    * Document/ File support for Microsoft Office documents are now available from our GitHub repo. Thanks to @chooklotto 
* Fuzzy Search for Quick Open has been vastly improved. It's now more accurate and speed is noticeably improved
* LightPaper now uses an alternative mechanism for sending feedback
* Real Preview: A default real preview site can be selected from within Real Preview preference
* You can now rate LightPaper so that we know how much you love it. Just a formality, we know it's always a 5 stars for you :)
* `Styles` menu item is now renamed to more appropriate `Document` menu
* Improved relative path rendering for images
* Always render local images with full paths regardless of document's base URL
* Make auto scrolling sync setting persistent
* Added a preference to allow/disallow adding an untitled document automatically
* Added a preference to turn off auto expanding a folder when adding it to sidebar
* Update the title of an already opened document's tab when the document is renamed
* Auto bulleting for nested lists
* PNGs and JPEGs are not filtered out by default from the folder navigator
* Lots of other minor improvements

#### BUG FIXES
* Cannot select a document if it is hidden in the overflow tabs menu (when there are too many tabs open)
* Type through autopair character if it is typed i.e. no more []] or ())
* Other few minor bug fixes
* Extra whitespace breaks Jekyll FrontMatter
* Multiple copies of LightPaper Mini is open in some cases
* Fixed a possible memory leak
* Cursor color is invisible when switching from Solarized Light theme to LightPaper Dark
* App crashes when hitting enter on quick search when there are no results
* Cursor and text jump when opening a document
* Few other minor bug fixes

Thanks a lot to all our beta testers who made this release as much bug free as possible. You guys are awesome! 👍 