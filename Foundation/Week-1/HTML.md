
# W01 - D02 - [HTML tags](https://html.com/tags/)

## `<head>` - head
- Container for all the head elements.
- Contains metadata only, like title for the document, scripts, styles, meta information, and more.
- Connecting to some file, give title, etc ...
- It is so that the document works as it is supposed to
- _(The browser reads the file from the top, so if you put the link (to css for example) to the bottom, until you reach it, the linked css will not get applied)_


#### The following elements can go inside the <br/>`<head>`
- `<title>` (this element is **required** in an HTML document)
- `<style>`
- `<base>`
- `<link>`
- `<meta>`
- `<script>`
- `<noscript>`

```HTML
<head>
  <meta charset="utf-8">
  <link rel="stylesheet" href="style.css" type="text/css">
  <title>First</title>
</head>
```

### `<body>` - BODY
- Defines the document's body.
- Contains all the contents of an HTML document, such as text, hyperlinks, images, tables, lists, etc.
- Here comes everything that gets visible on the HTML page


### `<main>` - MAIN CONTENT
- Used to denote the content of a webpage that relates to the central topic of that page or application.


```HTML
<main>
   <article>
       <p>This is the first.</p>
       <p>This is the second.</p>
   </article>
   ...
</main>
```


### `<article>` - ARTICLE
- Identifies a self-contained piece of content which could theoretically be distributed to other websites and platforms as a stand-alone unit.
- It is a good choice to contain entire blog posts, news articles, and similar content.

```HTML
<article>
    <p>This is the first paragraph.</p>
    <p>This is the second paragraph.</p>
</article>
```

### `<h1 ...6 >` - HEADING
- A heading element implies all the font changes, paragraph breaks before and after, and any white space necessary to render the heading.
- HTML defines six levels of headings --> H1, H2, H3, H4, H5, and H6
- H1 --> importance --> H6

<h1> H1</h1>
<h2> H2</h2>
<h3> H3</h3>
<h4> H4</h4>
<h5> H5</h5>
<h6> H6</h6>

```HTML
<h1>Favorites</h1>
<h2>Favorite notations</h2>
```

### `<p>` - PARAGRAPH
Used to identify blocks of paragraph text.

```HTML
<p>Always code as if the guy who ends up maintaining your code will be a violent psychopath who knows where you live.</p>
```

### `<div>` - (BLOCK) SECTION
Defines an arbitrary block of content which can be placed and styled as a single unit. It has no particular semantic meaning: it simply defines a block of content which can be styled as a single unit on a page.

```HTML
<div>
  <h2>Favorite links</h2>
  <a href="http:\\www.greenfoxacadem.com">GFA</a>
</div>
```

### `<span>` - (INLINE) SECTION
The inline equivalent to the block-level <div> element. It is used to select inline content for purely stylistic purposes.

```HTML
<p>My mother has <span>blue</span> eyes.</p>
```

### `<strong>` - EMPHASIZED TEXT
Used to identify text that is of greater importance than the surrounding text. <br/>
By default, all browsers render <strong> text in a bold typeface.

```HTML
<strong>Strong text</strong>
```

### `<a>` - HYPERLINK / ANCHOR
Used to create a hyperlink to another webpage or another location within the same webpage. <br/>
The hyperlink created by an anchor element is applied to the text, image, or other HTML content nested between the opening and closing <a> tags.

```HTML
<a href="http:\\www.greenfoxacademy.com">GFA</a>
```

### `<img>` - IMAGE
Used to insert an image into a document. All `<img>` tags must have a defined src attribute. 

Available image formats are the most common ones: JPEG, [GIF] including animated GIFs, PNG, APNG, SVG, BMP <br/>
Alt: alternative text (provided the image cannot be loaded)

```HTML
<img src="flower.gif" alt="missing">
```

### `<nav>` - NAVIGATION
Identifies a group of navigation links. Links in a <nav> element may point to other webpages or to different sections of the same webpage.

```HTML
<nav>        
  <a href="http:\\www.whatever.hu">KD</a>
  <a href="http:\\www.greenfoxacadem.com">GFA</a>
  <a href="http:\\www.index.hu">Index</a>
</nav>
```

### `<ol>` and `<ul>` ORDERED LIST, UNORDERED LIST
- ol --> defines an ordered list. An ordered list can be numerical or alphabetical.
- ul --> defines an unordered (bulleted) list.


Use the `[<li>]` tag to define list items for both of them

```HTML
<ol>
     <li class="firstItem">Dog</li>
     <li>Dog</li>
     <li>Fox</li>
     <li>Cat</li>
</ol>
```