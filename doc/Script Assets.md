[LightPaper](http://lightpaper.42squares.in/?ref=foo) version 1.2 introduces new feature that allows you to add any local or remote JavaScript or CSS assets. This might sound simple and trivial but it opens a lot of possibilities what you can do with LightPaper now. Think of it as a "plugin" feature for LightPaper powered by JavaScript and CSS.

### So what does it do really?
How about adding [flowcharts](https://en.wikipedia.org/wiki/Flowchart), [sequence diagrams](https://en.wikipedia.org/wiki/Sequence_diagram) and [gantt charts](https://en.wikipedia.org/wiki/Gantt_chart) to your documents using nothing more than just plain text? Check out this document for more details: [Mermaid + LightPaper = ❤️](https://github.com/42Squares/LightPaper/blob/master/doc/Adding%20Mermaid%20Diagrams.md)

Seriously? Yep!

### Adding a new asset
Adding a new asset is a piece of cake:

1. Go to `Preferences...>Script Assets` (if it is hidden, click on the `>>` button)
2. Click on the `+` button and add a local or remote URL for your asset in **File Source** field, give it a name and click `Add`.

That's it!

Seriously? Yep!

Assets are loaded in the order they appear on the table. You can select multiple assets and drag-and-drop them to change the order and can even enable or disable them.

![](https://raw.githubusercontent.com/42Squares/LightPaper/master/screenshots/scriptAssetsPref.png)

In the above screenshot you can notice that there is a **On Update Callback Script** button. Here you can add any JavaScript code that gets called as soon as the preview is rendered. This allows you to write your own code to modify the output.

Script Assets brings a lot of possibilities to modify and add new features to your documents. Give it a try and let us know.

 