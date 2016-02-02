## Setting base URL for a document
`Added in version 1.3`

Setting a base URL determines how your local assets, such as images, will be rendered in [LightPaper][2]. It might look a little bit daunting at first but this is a very useful feature.

If you are editing/rendering a document from a folder and you have referenced images from a different folder, this is something you really want to know. This is also a useful feature if you are writing documents using static site generators such as [Jekyll][1].

### Understanding using an example

To make it easy to understand, we will set a fictitious folder structure:

	/Users/JaneDoe/Desktop/
		0.png
		DirectoryA/
		DirectoryB/
			docB.md
			B.png
			DirectoryB1
				B1.png
		DirectoryC/
			docC.md
			C.png
			
In the above fictitious folder structure, `DirectoryA`, `DirectoryB`, `DirectoryC` are all folders inside JaneDoe's `Desktop` folder.

Ok, now let's say `docB.md` has this content:

	![](/Users/JaneDoe/Desktop/0.png)
	
	![](0.png)
	
	![](B.png)

	![](DirectoryB1/B1.png)
	
	![](C.png)

As you can see, this document references **4 unique images** from **4 different locations** in **5 different ways**! If you have worked with referencing images in Markdown documents then you know the headache it brings. It's good to avoid this but practically it's not possible to just ignore it - unless you want to not have images rendered or unless you manually want to edit all your image references when you are ready to publish, which is definitely not ideal.

Ok, now let's see how [LightPaper][2]'s new `Document>Set Base URL` feature helps us to properly resolve these image references according to your needs.

### 1) Set document's base URL to: *`None`*

- [x]	 `![](/Users/JaneDoe/Desktop/0.png)` gets rendered

This makes sense - you basically said "No base URL" and the only one that gets rendered is the one with full path.

If you have set full path to your local file, [LightPaper][2] will **always** render it no matter which option you choose.

### 2) Set document's base URL to: *`Document's Parent Folder`*

- [x]	 `![](B.png)` gets rendered
- [x]	 `![](DirectoryB1/B1.png)` gets rendered
- [x]	 `![](/Users/JaneDoe/Desktop/0.png)` gets rendered

This makes sense too - you said "every thing is relative to this document's parent path" which is `/Users/JaneDoe/Desktop/B` and the images inside this folder, including sub-folders, get rendered.

Now the other 2 options are only available if you have opened a folder and have opened `docB.md` from the folder navigator. This is what you'd do if, say, you were using a [Jekyll][1] site. 

Let's assume that you have opened `/Users/JaneDoe/Desktop` folder and opened `docB.md` by double-clicking or by using [LightPaper][2]'s [Quick Open](http://lightpaper.42squares.in/#multitabs-container) feature.

### 3) Set document's base URL to: *`Sidebar's Root Folder`*

- [x]	 `![](0.png)` gets rendered
- [x] 	`![](/Users/JaneDoe/Desktop/0.png)` gets rendered

When you selected `Sidebar's Root Folder`, you set the base path to `/Users/JaneDoe/Desktop` and because `0.png` is inside `/Users/JaneDoe/Desktop` folder, it gets rendered. No rocket science, really!

### 4) From the sidebar, right-click on `DirectoryC`, select `Set as Base Folder` and set document's base URL to: *`Custom Folder from Sidebar`*

- [x] `![](C.png)` gets rendered
- [x] `![](/Users/JaneDoe/Desktop/0.png)` gets rendered

You set the path to `DirectoryC` and hence `C.png` gets rendered. This is really really useful if you are editing [Jekyll][1] files.

Also, as a convenience, [LightPaper][2] remembers your selected option for a document. So, once you set a base URL, you don't have to set it again.

| Image Path                              | Base URL Option            | Renders                          | Condition                                                                            |
|-----------------------------------------|----------------------------|----------------------------------|--------------------------------------------------------------------------------------|
| /Users/JaneDoe/Desktop/0.png            | None                       |  "/Users/JaneDoe/Desktop/0.png"  |                                                                                      |
| /Users/JaneDoe/Desktop/DirectoryB/B.png | Document's Parent Folder   | "B.png" and "DirectoryB1/B1.png" and "/Users/JaneDoe/Desktop/0.png" | |
| /Users/JaneDoe/Desktop/0.png            | Sidebar's Root Folder      | "0.png" and "/Users/JaneDoe/Desktop/0.png" | Document is opened from Folder Navigator                                             |
| /Users/JaneDoe/Desktop/DirectoryC/C.png | Custom Folder from Sidebar | "C.png" and "/Users/JaneDoe/Desktop/0.png" | Document is opened from Folder Navigator and DirectoryC is selected as a base folder |

You might have already figured it out -- yes, it's all about just setting relative path. If you are still finding it difficult, instead of trying to remember all these combinations, just try different options and see which one works. Very Soon everything starts making sense.

[1]: http://jekyllrb.com/
[2]: http://lightpaper.42squares.in/?ref=github