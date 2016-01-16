#### Mermaid + LightPaper = ❤️

## Adding diagrams to your documents using Mermaid and LightPaper

[Mermaid](http://knsv.github.io/mermaid/#mermaid) is a JavaScript library accompanied by couple of CSS files that allows you to add diagrams to your documents using Markdown like syntax. It's really pretty sleek.

With the introduction of `Script Assets` in [LightPaper version 2.0](https://github.com/42Squares/LightPaper/blob/master/WhatsNew/ver1.2.md), adding Mermaid documents in your documents is a piece of cake. These are the initial and "one time only" steps required:

1. Go to `Preferences...>Script Assets` (if it is hidden, click on the `>>` button)
2. Click on the `+` button and add `https://cdnjs.cloudflare.com/ajax/libs/mermaid/0.5.6/mermaid.min.js` for **File Source** and `Mermaid JS` for **Name** and click `Add`.
3. Click on the `+` button again and add `https://cdnjs.cloudflare.com/ajax/libs/mermaid/0.5.6/mermaid.forest.min.css` for **File Source** and `Mermaid CSS` for **Name** and click `Add`.
4. Click on `+ On Update Callback Script` and add `mermaid.init(null, '.mermaid');` and click `Save`.

That's it! You are all set!!

Now let's add some diagrams using Mermaid syntax:

### Flowchart example:

```html
<div class="mermaid">
    graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
</div>
```
You should see something like this:
![](https://raw.githubusercontent.com/42Squares/LightPaper/master/screenshots/mermaid_sample_1.png)

### Sequence Diagram example:

```html
<div class="mermaid">
    sequenceDiagram
      participant Alice
      participant Bob
      Alice->John: Hello John, how are you?
      loop Healthcheck
        John->John: Fight against hypochondria
      end
      Note right of John: Rational thoughts <br/>prevail...
      John-->Alice: Great!
      John->Bob: How about you?
      Bob-->John: Jolly good!
</div>
```

You should see something like this:
![](https://raw.githubusercontent.com/42Squares/LightPaper/master/screenshots/mermaid_sample_2.png)

Cool, huh?

These are just couple of simple examples. You can write more advanced and complex diagrams using Mermaid's simple Markdown like syntax. Like adding [Font Awesome]() icons. Visit their website: http://knsv.github.io/mermaid/#mermaid for more information and examples.

Also, you can find other CSS styles and the latest versions of Mermaid here: https://cdnjs.com/libraries/mermaid


## Alternate Mermaid Syntax
If you're one of those who doesn't like adding html elements, like `<div class="mermaid">` above, to your Markdown documents then there is a better way. You can teach LightPaper to allow you to use familiar [GitHub fenced code blocks syntax](https://help.github.com/articles/github-flavored-markdown/#fenced-code-blocks):

1. Go to `Preferences...>Script Assets` (if it is hidden, click on the `>>` button)
2. Click on `+ On Update Callback Script` and append `mermaid.init(null, '.language-mermaid');` and click `Save`.

That's it!

Now let's add a Flowchart using fenced code syntax:

```html
 ```mermaid
       graph TD;
         A-->B;
         A-->C;
         B-->D;
         C-->D;
 ```
```

If you see some weird whitespace and ugly background color, you can add following global styles in `Preferences...>Custom CSS` (thanks [@mmatti](https://twitter.com/mmatti)):

```css
pre.language-mermaid, code.language-mermaid{ 
  color:inherit !important; 
  background-color:inherit !important; 
  font-family:inherit !important; 
} 

pre.language-mermaid > div {
  display: none;
}
```