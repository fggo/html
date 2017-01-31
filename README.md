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
	<dd>Coffee is a brewed drink prepared from roasted coffee beans, which are the seeds of berries from the Coffea plant.</dd>
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
