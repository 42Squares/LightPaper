## What's new in LightPaper version 1.4.x Alpha?

#### FEATURES

* **Plugins** -  Starting with 1.4 you'll be able to write plugins for LightPaper using CocoaScript, the same framework that powers Sketch app. For more info, [watch our dedicated plugins repo](https://github.com/42Squares/LightPaperPlugins)
* **Snippets** - You can now create snippets `File>New Snippet...` and use it later locally. Use *@<snippet_name>* to add snippet as it is or *@<snippet_name>.h* to insert HTML version of the snippet.
* **Sorting Sidebar Items** - You can now sort sidebar items (except Folders) using different options. Right-click on one of the FAVORITES, SCRATCH NOTES, SHADOW NOTES headers for Sorting Options.
* You can now use shortcuts to jump between editor and the sidebar. See `View > Jump to Sidebar` and `View > Jump to Editor` for available shortcuts.
* You can now use CMD+ENTER to open a sidebar item instead of using your mouse and double clicking it.
* New unsaved files are restored automatically when closing the application without asking you to save first. If you close a tab, however, you'll be prompted to save first if it is unsaved.
* Added a new syntax highlighting theme - Solarized.
* One click document open. Save yourself a click as you don't have to double click to open a document. Single click will temporarily open a document. To permanently open a click, double click like usual.
* One click folder toggle. A single click will expand/ collapse a folder in the navigator.
* LightPaper Mini - added a slider to change the width/height ratio of the mini popover window. This can be accessed from the preferences.


We'll be adding more documentation about Plugins and Snippets on our official LightPaper GitHub project: https://github.com/42Squares

#### IMPROVEMENTS 
* LightPaper now always remembers opened folder not just when restarting the app.
* Don't autobullet if ENTER is done at the beginning of the line
* When trying to open a folder, focus it instead if it is already opened
* LightPaper now remembers the order of files when restoring them.
* Added a "Close All Tabs" menu item
* A document's base URL is always set to its parent folder by default
* Editor outline now recognizes --- and === tags for headers as well
* Syntax highlight now supports more languages out of the box including SQL
* Scratch and Shadow notes are not restored as well when opening the app.
* Scratch and Shadow notes are automatically saved when closing the app.
* App will now remember your expanded folders when from previous session.
* Changed the placements of both editor outline and preview outline

#### BUG FIXES
* Fixed a bug the app would crash on closing if there is at least one unsaved document
* Fixed navigator jumpiness when opening a document
* Fixed a bug where sometimes multiple copies of LightPaper would run
* Fixed a bug where distraction free mode would show a white border when using a dark theme
* Other few minor bugfixes