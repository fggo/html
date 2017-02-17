* [Structure] (https://github.com/fggo/html/blob/master/README.md#structure)
* [Text] (https://github.com/fggo/html/blob/master/README.md#text)
* [Semantic Markup] (https://github.com/fggo/html/blob/master/README.md#semantic-markup)
* [Lists] (https://github.com/fggo/html/blob/master/README.md#lists)
* [Links] (https://github.com/fggo/html/blob/master/README.md#links)
* [Images] (https://github.com/fggo/html/blob/master/README.md#images)
* [Table] (https://github.com/fggo/html/blob/master/README.md#table)
* [Forms] (https://github.com/fggo/html/blob/master/README.md#forms)
* [Extra markup] (https://github.com/fggo/html/blob/master/README.md#extra-markup)

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
<!--Block quote-->
<blockquote cite = "https://en.wikipedia.org/wiki/Floyd_Mayweather_Jr."> 
	<p>Easy Work.</p> 
</blockquote>

<!--Quotation mark: does not work in IE-->
<q>Fly like a butterfly. Sting like a bee.</q>
```

### Abbreviation
```html
<abbr title = "Professor">Prof</abbr> will discuss the topic.
```

### Acronym
```html
<acronym title = "President Of The United States">POTUS</acronym> is flying.
```

### Citation
```html
<!--cite-->
<cite>A Brief History of Time</cite> by Stephen Hawking has sold over ten million copies worldwide.
```

### Definitions
```html
<!--dfn-->
<dfn>Black hole</dfn> is a region of space from which nothing, not even light, can escape.
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
<p>It was the <del>worst</del>  <ins>best</ins> decision I'd ever made
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
```html
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
```

## Links

### Absolute and Relative URL
* Abosolute URL : domain name for a site followed by the path to a specific page
* Relative URL: link to other pages within the same site
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
Web servers usually set up to return the index.html file. examplearts.com will return examplearts.com/index.html
```

root folder contains:

* a file called index.html, homepage
* folders for movie, music, theatre

each sub-dir contains:

* index.html, homepage for that section
* reviews.html
* listings.html except DVD dir

movie dir contains 

* cinema folder
* DVD folder

### Relative URL
```
when you link to a page on your own website, you do not need to specify the domain name.
instead you can use relative URLs.
```

cur dir
```html
<a href = "reviews.html">Reviews</a>
```

child dir
```html
<a href = "music/listings.html">Listings</a>
<a href = "movies/dvd/reviews.html">Reviews</a>
```

parent dir
```html
<a href = "../index.html">Home</a>
<a href = "../../index.html">Home</a>
```

### Email Links
```html
<!--mailto:-->
<a href = "mailto:jon@example.org">Email Jon</a>
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
absolute or relative URL, followed by the value of the id attr
<a href = "http:/www.htmlandcssbookcom/#bottom">book</a>
```

## Images
```html
<!--src: relative url-->
<!--alt: desc that shows up if image is broken-->
<!--title: info when mouse cursor hover-->
<!--height width: size-->
<!--specify img size to make page load faster -->
<!--img placement can be changed around paragraph-->
<p>
	<img 
	src = "../Pictures/astronaut.jpg"
	alt ="NASA astronaut lands on moon for the first time in human history"
	title = "Astronaut"
	height = "200"
	width = "110">
</p>
```

### img align [old code]
```html
'align' attr is no longer used in HTML5.
new website should use CSS to control alignment of images.
<!--left, right-->
<p>
	<img 
	src = "work.jpg" alt ="stretches before workout" title = "work" height = "100" width = "150"
	align = "left">Working out is essential for people who works on the desk daily.
	<img 
	src = "work.jpg" alt ="stretches before workout" title = "work" height = "100" width = "150"
	align = "right">Working out is essential for people who works on the desk daily.
</p>
<!--top, middle, bottom (first line)-->
<p>
	<img 
	src = "puma.jpg" alt ="in nature" title = "puma" height = "100" width = "180"
	align = "top">Puma is a big cat.
	<img 
	src = "puma.jpg" alt ="in nature" title = "puma" height = "100" width = "180"
	align = "middle">Puma is a big cat.
	<img 
	src = "puma.jpg" alt ="puma in nature" title = "puma" height = "100" width = "180"
	align = "bottom">Puma is a big cat.
</p>
```

### Rules for creating img
1. img in right format (jpeg gif png)
2. img in right size
3. img in correct resolution (72 px)

### Tools to edit img
1. Adobe Photoshop
2. GIMP
4. Blender
5. Abobe Fireworks
6. Pixelmator
7. PaintShop Pro
8. Paint.net

### jpeg
use .jpeg for img with many different colors

### gif png
use .gif or .png for img with few colors or large areas of the same color

## img dimension
reduce, increase, change shapes of a img

### img resolution
```html
img for web should be saved at a resolution of 72 ppi
bitmap format : JPG, GIF, PNG
```

### Vector img
differs from bitmap image and resolution-independent<br/>
commonly created with Adobe Illustrator<br/>
place points on a gird and draw lines between them and color can be fill in<br/><br/>
The current method of using vector images for display on websites <br/>
involves saving bitmap version of the original vector images and using that. <br/>

### Animated gifs
shows several frames of an image in sequence to create simple animations
due to increasing file sizes, gif is only suitable for simple illustration

### Transparency
creating a partially transparent img for web involves selecting one of two formats :
* transparent gif : straight edged img
* png : diagonal, round, semi-opaque, drop-shadow img


### figure figcaption
To contain both img and caption
```html
<figure>
	<img src = "../../Pictures/astronaut.jpg"  alt = "astronaut standing on the moon">
	<img src = "../../Pictures/astro2.jpg" alt = "astronaut saying hello">
	<br/>
	<figcaption>
		HTML5 allows caption for multiple images
	</figcaption>
</figure>
```

## Table

### table heading
<!--th: heading for row or col-->
<table border =1>
	<tr>
		<th></th>
		<th scope = "col">SAT</th>
		<th scope = "col">SUN</th>
	</tr>
	<tr>
		<th scope = "row">Tickets sold:</th>
		<td>120</td>
		<td>135</td>
	</tr>
	<tr>
		<th scope = "row">Total sales:</th>
		<td>$600</td>
		<td>$675</td>
	</tr>
</table>


### spanning columns
```html
colspan can be used on <td> or <th>
<table border =1>
	<tr>
		<td colspan ="2">A</td>
		<td colspan ="2">B</td>
	</tr>
	<tr>
		<th colspan ="4">C</th>
	</tr>
</table>
```

### spanning rows
```html
<table border = 1>
	<tr>
		<td rowspan ="2">A</td>
		<td>B</td>
	</tr>
	<tr>
		<td>C</td>
	</tr>
</table>
```

### thead tbody tfoot
in case of long table, thead tbody tfoot allow header and footer visible allowing scrolls in body
```html
<table border = "1">
	<thead>
		<tr>
			<th>Data</th>
			<th>Income</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<th>1st Jan</th>
			<td>10</td>
		</tr>
		<!--2-30 Jan-->
		<tr>
			<th>31st Jan</th>
			<td>10</td>
		</tr>
	</tbody>
	<tfoot>
		<tr>
			<td></td>
			<td>120</td>
		</tr>
	</tfoot>
</table>
```

### Width & spacing [old code]
```html
replaced with CSS
<!--width: table width-->
<!--cellpadding: space inside each cell-->
<!--cellspacing: space between each cell-->
<table width ="400" cellpadding = "10" cellspacing = "5" border = "1">
	<tr>
		<th width ="150"> </th>
		<th>withdrawn</th>
		<th>credit</th>
		<th width ="150">balance</th>
	</tr>
	<tr>
		<th>January</th>
		<th>250</th>
		<th>600</th>
		<th>400</th>
	</tr>
</table>
```

### Border & background [old code]
```html
<table border ="2" bgcolor = "#efefef">
	<tr>
		<th width = "150"></th>
		<th>withdrawn</th>
		<th>cefdit</th>
		<th width = "150" bgcolor = "#cccccc">balance</th>
	</tr>
	<tr>
		<th>January</th>
		<td>250.00</td>
		<td>660.50</td>
		<td bgcolor = "#cccccc">410.50</td>
	</tr>
</table>

```

## Forms

### Form control

### adding text
1. text input (single line)
2. pw input
3. text area

### making choices
1. radio btn
2. checkboxes
3. drop-down boxes

### how forms work
1. user fills in a form and press submit btn
2. name and value pair of each form control is sent to the server
3. server processes info using lang like PHP, C#, VB.net, Java and stores info in a database.
4. server creates a new page to send back to the brower based on the info received

### form structure
1. action: url for the page on the server receiving submitted info
2. method : get(action url + form val added at the end)<br/> post(val is sent in what are known as HTTP headers)
  * get: short forms (such as search boxes)
  * get: when retrieving data from web server, not sending info that <br/> should be added to or deleted from database
  * get:  default (when method attr is not used)

  * post: forms that allow users to upload a file
  * post: long forms
  * post: containing sensitive data (pw)
  * post: forms that add or delete info from a database
3. id: identify the form distinctly from other elements on the page

```html
<form action = "http://www.example.com/subscribe.php" method = "get">
	<p>This is where the form controls will appear</p>
</form>
```

### input
```html
<!--name: each form control needs name attr-->
<!--size: num of char [old forms: CSS]-->
<form action = "http://www.example.com/login.php" method = "get">
	<p>username: 
		<input type = "text" name = "username" size = "15" maxlength = "30" />
	</p>
	<p>password: 
		<input type = "password" name = "password" size = "15" maxlength = "30" />
	</p>
</form>
```

### textarea
```html
<form action = "http://www.example.com/comments.php" method = "get">
	<p>What do you think of  this gig</p>
	<textarea name = "comments" cols = "20" rows = "4">Enter your comments</textarea>
</form>
```

### radio btn
```html
<!--checked: which val should be selected when page loads-->
<form action = "http://www.example.com/profile.php">
	<p>Please select your favorite genre</p>
	<br/>
	<input type = "radio" name = "genre" value = "rock" checked = "checked"/> Rock
	<input type = "radio" name = "genre" value = "pop"/> Pop
	<input type = "radio" name = "genre" value = "jazz"/> Jazz
</form>
```

### checkbox
```html
<form action = "http://www.example.com/profile.php">
	<p>Please select your favorite music service(s)</p>
	<br/>
	<input type = "checkbox" name = "service" value = "itunes" checked = "checked"/> iTunes
	<input type = "checkbox" name = "service" value = "lastfm"/> Last.fm
	<input type = "checkbox" name = "service" value = "spotify"/> Spotify
</form>
```

### dropdown list box
```html
<!--select: it creates drop down list which allows users to select one val-->
<!--selected: default selected when page loads. if not used, the first is selected-->
<form action = "http://www.example.com/profile.php">
	<p>What device do you listen to music on?</p>
	<select name = "devices">
		<option value = "ipod" selected = "selected">iPod</option>
		<option value = "radio">Radio</option>
		<option value = "computer">Computer</option>
	</select>
</form>
```

### multiple select box
```html
<form action = "http://www.example.com/profile.php">
	<p>Play any Instruments? (multi select available)</p>
	<select name = "instruments" size = "3" multiple = "multiple">
		<option value = "guitar" selected = "selected">Guitar</option>
		<option value = "drums">Drums</option>
		<option value = "keyboard">Keyboard</option>
		<option value = "bass">Bass</option>
	</select>
</form>
```

### file input box
```html
<form action = "http://www.example.com/upload.php" method = "post">
	<p>upload your song in mp3 format</p>
	<input type = "file" name = "user-song"/> <br />
	<input type = "submit" value = "Upload"/>
</form>
```

### submit btn
```html
<!--value: text that appears on the page-->
<form action = "http://www.example.com/subscribe.php">
	<p>subscribe to our email list:</p>
	<input type = "text" name = "email"/>
	<input type = "submit" name = "subscribe" value = "Subscribe"/>
</form>
```

### image btn
```html
<!--alt works as used in <img>-->
<form action = "http://www.example.com/subscribe.php">
	<p>subscribe to our email list:</p>
	<input type = "text" name = "email"/>
	<input type = "image" src = "subscribe.png" width = "100" height ="20"/>
</form>
```

### button & hidden controls
```html
<!--input hidden: allow page authors to add val to forms users can't see-->
<!--author might use hidden field to indicate which page the user was on when submitting a form-->
<form action = "http://www.example.com/add.php">
	<button><img src = "add.gif" alt = "add" width = "10" height = "10"/>Add</button>
	<input type = "hidden" name = "bookmark" value = "lyrics"/>
</form>
```

### labelling form controls
1. wrap around text and form input 
2. separate form form and use 'for' to indicate which form to label
```html
<label>Age: <input type = "text" name = "age"/></label><br/> 

Gender:
<input id = "female" type = "radio" name = "gender" value = "f">
<label for = "female">Female</label>
<input id = "male" type = "radio" name = "gender" value = "m">
<label for = "male">Male</label>
```

### Grouping form elements
```html
<fieldset>
	<legend>Contact details</legend>
	<label>Email:<br/><input type = "text" name = "email"/></label>
	<label>Mobile:<br/><input type = "text" name = "mobile"/></label>
	<label>Tel:<br/><input type = "text" name = "tel"/></label>
</fieldset>
```

### HTML5: form validation
validate contents of the form before sent to the server. traditionally javascript 
```html
<form action = "http://www.example.com/login/" method = "post">
	<label for "username">Username:</label>
	<input type = "text" name = "username" required = "required"/><br/>
	<label for "password">Password:</label>
	<input type = "password" name = "password" required = "required"/>
	<input type = "submit" value  = "Submit"/>
</form>
```

### HTML5: date input
```html
<form action = "http://www.example.com/bookings/" method = "post">
	<label for = "username">Departure date:</label>
	<input type = "date" name = "depart"/>
	<input type = "submit" value = "Submit"/>
</form>
```

### HTML5: email & url input
```html
<form action = "http://www.example.org/subscribe.php">
	<p>Please enter your email address:</p>
	<input type = "email" name = "email"/>
	<input type = "submit" value = "Submit"/>
</form>

<form action = "http://www.example.org/profile.php">
	<p>Please enter your website address:</p>
	<input type = "url" name = "website"/>
	<input type = "submit" value = "Submit"/>
</form>
```

### HTML5: search input
```html
<form action = "http://www.example.org/search.php">
	<p>Search:</p>
	<input type = "search" name = "search"/ placeholder = "Enter keyword">
	<input type = "submit" name = "submit"/>
</form>
```

## Extra markup

### The Evolution of HTML
HTML4<br/>
XHTML 1.0 follow the rule of XML<br/>s
HTML5

### DOCTYPE
to tell a browser which vedrsion of HTML the page is using and render page correctly<br/>
HTML5
```html
<!DOCTYPE html>
```

HTML4
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Traditional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```

Traditional XHTML 1.0
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Traditional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-traditional.dtd">
```

Strict XHTML 1.0
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
```

XML Declaration
```html
<?xml version = "1.0" ?>
```

## id
