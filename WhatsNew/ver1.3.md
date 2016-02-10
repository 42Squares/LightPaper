## What's new in LightPaper version 1.3 Beta?

#### FEATURES ✨

* **Multiple Folders** -  📂🗄So many users have asked for this!!! Sidebar now supports multiple folders. Add as many as you want or remove the ones you don't want.
* **Editor Outline Navigator** - 🗺 Quickly navigate between your headers or code blocks. [Learn more...](https://www.youtube.com/watch?v=pvKF7G_E304)
    * Two-way navigation for editor outline navigator - clicking a header navigates to corresponding preview header as well.
	* Preview Outline is rewritten from scratch - looks better and supports two-way navigation as well
* LightPaper Mini: Added a preference to automatically insert shadow note's source path or URL
* Select markdown text and copy it as rich formatted text including images
* Select markdown text and copy them as HTML
* Added a top-level Export menu for quickly accessing exporting and copying features
* LightPaper now adds different ways of setting the base URL for a document. [Learn more...](https://github.com/42Squares/LightPaper/blob/master/doc/Setting%20Document%20Base%20URL.md)

#### IMPROVEMENTS

* LightPaper now re-renders your document when you make any changes to your sidebar's root folder(s). This makes it to render your new/modified images without having to restart LightPaper, for an example 🖼.
* **LightPaper Mini**:
    * Save mini documents when app gets inactive
    * `⌘+S` now continues to save a scratch or shadow note instead of persisting it to a file. You can save it to a file using `File>Save to File...` menu item or using `⌘+⌥+S` key.
    * Shadow Notes now by default selects the active tab for both Chrome and Safari.
    * Sync open notes between LightPaper and LightPaper Mini
    * Don't collapse expanded shadow notes when switching tabs or deleting a note
* Fuzzy Search for Quick Open has been vastly improved. It's now more accurate and speed is noticeable
* LightPaper now uses an alternative mechanism for sending feedback
* Real Preview: A default real preview site can be selected from within Real Preview preference
* Allow to rate LightPaper
* `Styles` menu item is now renamed to more appropriate `Document` menu
* Improved relative path rendering for images
* Always render local images with full paths regardless of document's base URL
* Make auto scrolling sync setting persistent
* Added a preference to allow/disallow adding an untitled document automatically
* Added a preference to turn off auto expanding a folder when adding it to sidebar
* Update the title of an already opened document's tab when the document is renamed
* Auto bulleting for nested lists
* PNGs and JPEGs are not filtered out by default from the folder navigator

#### B🐞G FIXES

* Type through autopair character if it is typed i.e. no more []] or ())
* Other few minor bug fixes
* Extra whitespace breaks Jekyll FrontMatter
* LightPaper Mini: Multiple copies of app is open in some cases
* Fixed a possible memory leak
* Cursor color is invisible when switching from Solarized Light theme to LightPaper Dark
* App crashes when hitting enter on quick search when there are no results
* Cursor and text jump when opening a document
