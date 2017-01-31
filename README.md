* [Structure] (https://github.com/fggo/html/blob/master/README.md#structure)
* [Text] (https://github.com/fggo/html/blob/master/README.md#text)
* [Semantic Markup] (https://github.com/fggo/html/blob/master/README.md#semantic-markup)
* [Lists] (https://github.com/fggo/html/blob/master/README.md#lists)
* [Links] (https://github.com/fggo/html/blob/master/README.md#links)

## Structure
```html
<html>
	<head> <!--info about page-->
		<title>web page title</title>
	</head>
	<body> <!--main browser window-->
		<h1>heading</h1>
		<p>paragraph</p>
		
		<h2>sub-heading</h2>
		<p>paragraph</p>
	</body>
</html>
```
## Text

### Bold
```html
<p>
	<b>bold</b> text
</p>
```

### Italic
```html
<p>
	<i>italic</i> text
</p>
```

### Superscript Subscript
```html
<p>
	E = MC<sup>2</sup> 
	H<sub>2</sub>O
</p>
```

### White space
```html
<!--two or more spaces collapse to one-->
<p>Hello World</p>
<p>Hello     World</p>
```

### Line breaks
```html
<p>Line One<br/>Line Two<br/>Line Three<br/></p>
```

### Horizontal rules
```html
<p>Current Topic</p>
<hr/>
<p>Next Topic</p>
```

## Semantic markup
- text elements that are not intended to affect the structure of web pages

### Strong
```html
<p>
	<strong>Warning!</strong> This is a tiger cage.
</p>
```

### Emphasis
```html
<!--emphasis that subtly changes the meaning of a sentence-->
<p><em>I</em> think water is empty</p>
<p>I <em>think</em> water is empty</p>
<p>I think water is <em>empty</em></p>
```

### Quotation
```html
<!--block quote-->
<blockquote cite = "https://en.wikipedia.org/wiki/Floyd_Mayweather_Jr.">
	<p>Like I said before... Easy work!</p>
</blockquote>

<!--quotation mark-->
<p>Respect is earned. You have to 
	<q>work hard.</q>  
	<!--does not work in IE-->
</p>
```

### Abbreviation
```html
<p>
	<abbr title = "Professor">Prof</abbr> 
	Foo will discuss the topic.
</p>
```

### Acronym
```html
<p>
	<acronym title = "President Of The United States">POTUS</acronym> 
	will address soon.
</p>
```

### Citation
```html
<!--cite-->
<p>
	<cite>A Brief History of Time</cite> by Stephen Hawking 
	has sold over ten million copies worldwide.
</p>
```

### Definitions
```html
<!--dfn-->
<p>A
	<dfn>black hole</dfn> is a region of space 
	from which nothing, not even light, can escape.
</p>
```

### Author details
```html
<!--address contains contact details-->
<address>
	<p><a href = "mailto:homer@example.org"> homer@example.org</a> </p>
	<p>742 Evergreen Terrace, Springfield.</p>
</address>

```

### Changes to content
```html
<!--del ins-->
<p>It was the 
	<del>worst</del> 
	<ins>best</ins> 
	decision I'd ever made
</p>


<!--no longer relevant-->
<p><s>Price is $200</s></p>
<p>Now Price is $150</p>
```

## Lists

### Ordered Lists
```html
<ol>
	<li>Buy Kaby Lake CPU</li>
	<li>Buy 512GB SSD</li>
	<li>Buy U2414H monitor</li>
</ol>
```

### Unordered Lists
```html
<ul>
	<li>melon</li>
	<li>water</li>
	<li>egg</li>
	<li>beef</li>
</ul>
```

### Definition Lists
```html
<dl>
	<dt>Bread</dt>
	<dd>Bread is a staple food prepared from a dough of flour and water, usually by baking.</dd>

	<dt>Coffee</dt>
	<dd>Coffee is a brewed drink prepared from roasted coffee beans.</dd>
</dl>
```

### Nested Lists
<ul>
	<li>Mathematics</li>
	<li>English</li>
	<li>Programming Language</li>
		<ul>
			<li>Java</li>
			<li>HTML & CSS</li>
			<li>JavaScript</li>
			<li>Python</li>
			<li>C++</li>
			<li>PHP</li>
		</ul>
</ul>

## Links

### Absolute and Relative URL
```html
<p>Movie Reviews:
	<ul>
		<li><a href = "https://www.rottentomatoes.com/"> 
			Rotten Tomatoes</a></li>
		<li><a href = "http://www.imdb.com/?ref_=nv_home">
			IMDB</a></li>
		<li><a href = "http://www.rogerebert.com/">
			Roger Ebert</a></li>
	</ul>
</p>

<p>
	<ul>
		<li><a href = "index.html">Home</a></li>
		<li><a href = "about-us.html">About</a></li>
		<li><a href = "movie.html">Movies</a></li>
		<li><a href = "contact.html">Contact</a></li>
	</ul>
</p>
```

### Directory structure
```html
Web servers usually set up to return the index.html file.
Every page and every image on a website has a URL,
which is made up of the domain name followed by the 
path to that page or image.

Path to the homepage:
	www.examplearts.com/index.html
Path to the logo for the site:
	examplearts.com/images/logo.gif
```


> the root folder contains:
* a file called index.html, homepage for entire site
* folders for movie, music, theatre section of the site

> each sub-dir contains:
* index.html, homepage for that section
* reviews.html
* listings.html except DVD dir

> movies section contains 
* cinema folder
* DVD folder

### Relative URL
```
when you link to a page on your own website,
you do not need to specify the domain name.
instead you can use relative URLs.
```

* same dir
```html
<a href = "reviews.html">Reviews</a>
```

* child dir
```html
<a href = "music/listings.html">Listings</a>
```

* grandchild dir
```html
<a href = "movies/dvd/reviews.html">Reviews</a>
```

* parent dir
```html
<a href = "../index.html">Home</a>
```

* grandparent dir
```html
<a href = "../../index.html">Home</a>
```

### Email Links
```html
mailto:
<p>
	<a href = "mailto:jon@example.org">Email Jon</a>
</p>
```


### Open Links in new window
```html
<!--target-->
<a href = "https://www.youtube.com/" target = "_blank">Youtube</a>
```

### Link to same page
```html
<h1 id = "top">Film-Making Terms</h1>
<a href = "#arc_short">Arc shot</a>
<a href = "#interlude">Interlude</a>
<a href = "#prologue">Prologue</a>

<h2 id = "arc_short">Arc Shot</h2>
<p>a shot in which the subject is photographed by ...</p>

<h2 id = "interlude">Interlude</h2>
<p>a breif, intervening film scene or ...</p>

<h2 id = "prologue">Prologue</h2>
<p>a speech, preface, intro...</p>

<p><a href = "#top">Top</a></p>
```


### Link to different page
```html
same but href attr will contain the address for the page
(absolute or relative URL), followed by the value of the id attr
<a href = "http:/www.htmlandcssbookcom/#bottom">book</a>
```

## Images
