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
```html
<p>
	<b>bold</b> text
	<i>italic</i> text
</p>

<p>
	E = MC<sup>2</sup> 
	H<sub>2</sub>O
</p>


<!--white space : two or more spaces collapse to one-->
<p>Hello World</p>
<p>Hello     World</p>


<!--Line Breaks-->
<p>Line One<br/>Line Two<br/>Line Three<br/></p>


<!--Horizontal Rules-->
<p>Current Topic</p>
<hr/>
<p>Next Topic</p>


<!--strong-->
<p><strong>Warning!</strong> tiger cage</p>


<!--em-->
<!--emphasis that subtly changes the meaning of a sentence-->
<p>I <em>think</em> water is empty</p>
<p>I think water is <em>empty</em></p>


<!--block quote-->
<blockquote cite = "https://en.wikipedia.org/wiki/Floyd_Mayweather_Jr.">
	<p>I like said before... Easy work!</p>
</blockquote>


<!--quotation mark: does not work in IE-->
<p>Respect is earned. You have to 
	<q>work hard.</q>
</p>


<!--abbreviation & acronym-->
<p><abbr title = "Professor">Prof</abbr> 
	Foo will discuss the future of Bar.
</p>
<p><acronym title = "President Of The United States">POTUS</acronym> 
	will be attending the summit this month.
</p>


```


