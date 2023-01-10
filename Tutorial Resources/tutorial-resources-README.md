# Tutorial Resources Documentation
The aim of this documentation is to provide you with a basic sense of how to create each of the elements in a tutorial page.

To get started on your tutorial, you need to download the following files - 
- `template.html`
- `all.css`
- `template.css`
- `back.svg`

### Do not remove the following line in the HTML!!!

```HTML
<a id="back-button" href="tutorials.html"><img id="back" src="back.svg" alt=""></a>
```

as this line provides the "Back to Tutorials button", which is on every tutorial.

## Understanding the General structure of the HTML

If you've seen the tutorial on the Swinburne Pulsar Portal about "How to Create a Tutorial", then you'd recall that the general structure of each tutorial is the following - 

```HTML
<div class="tutorial">
  <a id="back-button" href="tutorials.html"><img id="back" src="back.svg" alt=""></a>
  <!-- Tutorial content here -->
</div>
<div class="footer">
  <p>&copy; 2023. The ARC Centre of Excellence for Gravitational Wave Discovery (OzGrav). Designed and Developed by Rudra Sekhri</p>
  <div class="orgs">
      <div class="cell" id="cell-1"><a href="https://www.ozgrav.org"><img src="ozgrav.png" alt="OzGrav"></a></div>
      <div class="cell" id="cell-2"><a href="https://www.swinburne.edu.au/"><img src="swinburne.jpg" alt="Swinburne"></a></div>
  </div>
</div>
```

**Please note!** Do not change this general structure of the tutorial as that will prevent the CSS from being applied to the correct elements.

## Getting Started

For every tutorial, there are the following elements - 

- Title
- Date
- Author

To create a title, just use the `<h1></h1>` to create you title, like so - 

```HTML
<div class="tutorial">
  <a id="back-button" href="tutorials.html"><img id="back" src="back.svg" alt=""></a>
  <h1>Title Here</h1>
</div>
```

The same can be done to add your author name, only instead of using the `<h1></h1>` tags, you will instead use the `<h2></h2>` tags.

Now, if you just typed your author name between the `<h2></h2>`, it wouldn't be in bold text. To make the name of the author (and for that matter any text), you must use the `<b></b>` HTML tags. E.g. - 

```HTML
<div class="tutorial">
  <a id="back-button" href="tutorials.html"><img id="back" src="back.svg" alt=""></a>
  <h2>By <b>Author Name Here</b></h2>
</div>
```

## Adding a paragraph

To add a paragraph, just insert the paragraph between the `<p></p>` HTML tags. E.g. - 

```HTML
<div class="tutorial">
  <a id="back-button" href="tutorials.html"><img id="back" src="back.svg" alt=""></a>
  <p>Here is a paragraph!</p>
  <p>Here is another paragraph with some <b>bold text!</b></p>
</div>
```

## Adding a subtitle

To add a subtitle, just insert the name of the subtitle between the `<h3></h3` HTML tags. E.g. -

```HTML
<div class="tutorial">
  <a id="back-button" href="tutorials.html"><img id="back" src="back.svg" alt=""></a>
  <h3>Here is a subtitle!</h3>
  <p>Here is a paragraph!</p>
  <h3>Here is another subtitle!</h3>
</div>
```

## Adding Images

To add an image, along with an associating caption, use the following structure inside the tutorial container (the `<div></div>` element with a class of "tutorial") - 

```HTML
<div class="tutorial">
  <a id="back-button" href="tutorials.html"><img id="back" src="back.svg" alt=""></a>
  <div class="image">
      <img src="source-to-image-here" alt="">
      <div class="description">
          <h3><i>Figure Title</i></h3>
          <p>Some text here./p>
      </div>
  </div>
</div>
```

## Adding Italic Text

If you noticed the previous example carefully, then you would've noticed the `<i></i>` tags. When text is put inside these HTML tags, the text becomes *italic*. You can use it for any text as follows - 

```HTML

<div class="tutorial">
  <a id="back-button" href="tutorials.html"><img id="back" src="back.svg" alt=""></a>
  <p>Here is a paragraph with <i>italic text</i></p>
  <h3>Here's a title with <i>italic text</i></h3>
</div>

```

## Adding Video

To add a video into your tutorial (a video that has been uploaded to YouTube), then all you need to do is - 

1. Go to the video you want to add
2. Click the share button
3. Click the embed button
4. Copy the HTML code and paste it into your HTML file (while also making sure that all that HTML code is inside the tutorial container)

## Adding Unordered Lists

To add unordered lists, then use the following HTML structure inside the tutorial container (the `<div></div>` element with a class of "tutorial") - 

```HTML

<div class="tutorial">
  <a id="back-button" href="tutorials.html"><img id="back" src="back.svg" alt=""></a>
  <ul>
      <li>Point one.</li>
      <li>Point two.</li>
      <li>Point three.</li>
    <!-- And so on... -->
  </ul>
</div>

```

## Adding Inline Links

Let's say you want to link your tutorial to some other webpage on the internet. To do that, you want to put the text that you want to act as the link inside the `<a></a>` tags. E.g. -

```HTML

<div class="tutorial">
  <a id="back-button" href="tutorials.html"><img id="back" src="back.svg" alt=""></a>
  <p>The link to this page can be found <a href="URL-to-page">here</a></p>
  <p><a href="URL-to-page-about-pulsars">Pulsars</a> are rapidly rotating neutron stars.</p>
</div>

```

