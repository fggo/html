* [Structure] (https://github.com/fggo/html/blob/master/README.md#structure)
* [Text] (https://github.com/fggo/html/blob/master/README.md#text)

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

### Bold Italic
```html
<p>
	<b>bold</b> text
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


### Line Breaks
```html
<p>Line One<br/>Line Two<br/>Line Three<br/></p>
```

### Horizontal Rules
```html
<p>Current Topic</p>
<hr/>
<p>Next Topic</p>
```

## Semantic Markup
> text elements that are not intended to affect the structure of web pages

### Strong
```html
<p>
	<strong>Warning!</strong> tiger cage
</p>
```

### Emphasis
```html
<!--emphasis that subtly changes the meaning of a sentence-->
<p>I <em>think</em> water is empty</p>
<p>I think water is <em>empty</em></p>
```

### Quotation
```html
<!--block quote-->
<blockquote cite = "https://en.wikipedia.org/wiki/Floyd_Mayweather_Jr.">
	<p>I like said before... Easy work!</p>
</blockquote>

<!--quotation mark-->
<p>Respect is earned. You have to 
	<q>work hard.</q>  
	<!--does not work in IE-->
</p>
```

### Abbreviation Acronym
```html
<p><abbr title = "Professor">Prof</abbr> 
	Foo will discuss the topic.
</p>
<p><acronym title = "President Of The United States">POTUS</acronym> 
	will address soon.
</p>
```

### Citation Definitions
```html
<!--cite-->
<p><cite>A Brief History of Time</cite> by Stephen Hawking 
	has sold over ten million copies worldwide.
</p>


<!--dfn-->
<p>A <dfn>black hole</dfn> is a region of space 
	from which nothing, not even light, can escape.
</p>
```

### Author Details
```html
<!--address contains contact details-->
<address>
	<p>
		<a href = "mailto:homer@example.org"> 
		homer@example.org</a>
	</p>
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


<!--s-->
<p>
	<s>Price is $200</s>
</p>
<p>Now Price is $150</p>
```

## Lists
