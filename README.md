* [Structure] (https://github.com/fggo/html/blob/master/README.md#structure)
* [Text] (https://github.com/fggo/html/blob/master/README.md#text)
* [Semantic Markup] (https://github.com/fggo/html/blob/master/README.md#semantic-markup)
* [Lists] (https://github.com/fggo/html/blob/master/README.md#lists)
* [Links] (https://github.com/fggo/html/blob/master/README.md#links)
* [Images] (https://github.com/fggo/html/blob/master/README.md#images)
* [Table] (https://github.com/fggo/html/blob/master/README.md#table)
* [Forms] (https://github.com/fggo/html/blob/master/README.md#forms)
* [Extra markup] (https://github.com/fggo/html/blob/master/README.md#extra-markup)
* [Flash Video Audio] (https://github.com/fggo/html/blob/master/README.md#flash-video-audio)
* [CSS] (https://github.com/fggo/html/blob/master/README.md#css)
* [Color] (https://github.com/fggo/html/blob/master/README.md#color)
* [Text] (https://github.com/fggo/html/blob/master/README.md#textcss)
* [Boxes] (https://github.com/fggo/html/blob/master/README.md#boxes)

## Structure
```html
<html>
	<head> <!--page info-->
		<title>web page title</title>
	</head>
	<body> <!--main browser window-->
		<h1>heading</h1>
		<p>paragraph</p>
	</body>
</html>
```
## Text

### Bold Italic
```html
<b>bold</b>
<i>italic</i>
```

### Superscript Subscript
```html
E = MC<sup>2</sup> 
H<sub>2</sub>O	
```

### White space
two or more spaces collapse to one
```html
<p>Hello     World</p>
```

### Line breaks
```html
Line One<br/>Line Two<br/>
```

### Horizontal rules
```html
<p>Current Topic</p>
<hr/>
```

## Semantic markup
Text elements that are not intended to affect the structure of web pages

### Strong
```html
<strong>Warning!</strong> This is a tiger cage.
```

### Emphasis
Emphasis that subtly changes the meaning of a sentence
```html
<p><em>I</em> think water is empty</p>
<p>I <em>think</em> water is empty</p>
<p>I think water is <em>empty</em></p>
```

### Quotation
```html
<blockquote cite = "https://en.wikipedia.org/wiki/Floyd_Mayweather_Jr."> 
	<p>TMT</p> 
</blockquote>

<!--quotation mark-->
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
<cite>A Brief History of Time</cite> by Stephen Hawking has sold over ten million copies worldwide.
```

### Definitions
```html
<dfn>Black hole</dfn> is a region of space from which nothing, not even light, can escape.
```

### Author details
Address contains contact details
```html
<address>
	<p><a href = "mailto:homer@example.org"> homer@example.org</a> </p>
	<p>742 Evergreen Terrace, Springfield.</p>
</address>
```

### Changes to content
```html
<del>worst</del> <ins>best</ins> season.

<!--no longer relevant-->
<s>Price is $200</s><br/>
   Now Price is $150
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
		<li><a href = "https://www.rottentomatoes.com/">Rotten Tomatoes</a></li>
		<li><a href = "http://www.imdb.com/?ref_=nv_home">IMDB</a></li>
		<li><a href = "http://www.rogerebert.com/">Roger Ebert</a></li>
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
Web servers usually set up to return the index.html file.<br/>
examplearts.com will return examplearts.com/index.html

### Relative URL

```html
<a href = "reviews.html">Reviews</a>
<a href = "music/listings.html">Listings</a>
<a href = "movies/dvd/reviews.html">Reviews</a>
<a href = "../index.html">Home</a>
<a href = "../../index.html">Home</a>
```

### Email Links
```html
<a href = "mailto:jon@example.org">Email Jon</a>
```

### Links in new window
```html
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

<a href = "#top">Top</a>
```

### Link to different page
```html
absolute or relative URL, followed by the value of the id attr
<a href = "http:/www.htmlandcssbookcom/#bottom">book</a>
```

## Images
```html
<!--src: relative url-->
<!--alt: description that shows up if image is broken-->
<!--title: info when mouse cursor hover-->
<!--height: width: specify image size to make page load faster-->
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
'align' attr is no longer used in HTML5. Use CSS to control alignment of images
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

### Bitmap: jpeg gif png
* .jpeg for img with many different colors
* .gif .png for img with few colors or large areas of the same color

## img dimension
reduce, increase, change shapes of an image

### img resolution
image for web should have a resolution of 72 ppi<br/>

### Vector img
Differs from bitmap image and resolution-independent, commonly created with Adobe Illustrator<br/>
Place points on a gird and draw lines between them and color can be fill in<br/><br/>

### Animated gifs
Shows several frames of an image in sequence to create simple animations<br/>
Due to increasing file sizes, gif is only suitable for simple illustration

### Transparency
Creating a partially transparent image for web involves selecting one of two formats :
* transparent gif : straight edged img
* png : diagonal, round, semi-opaque, drop-shadow img


### figure figcaption
Contains both image and caption:
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
<table border =1>
	<tr>
		<th colspan ="2">A</td>
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
long table allows thead & tfoot visible while allowing scrolls in tbody.
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

### Table Width & Spacing [old code]
```html
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

### Table Border & Background [old code]
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
1. text input
2. pw input
3. text area

### making choices
1. radio btn
2. checkboxes
3. drop-down boxes

### how forms work
1. user fills in a form and press submit btn
2. (name, value) pair of each form control is sent to the server
3. server processes info using lang like PHP, C#, VB.net, Java and stores info in a database.
4. server creates a new page to send back to the brower based on the info received

### form structure
1. action: url for the page on the server receiving submitted info
2. method : [get, post]
  * get: short forms(e.g. search boxes) to get data from web server, <br/>not sending info that should be added to or deleted from database
  * post: long forms to upload a file or long forms
  * post: containing sensitive data (pw)
  * post: forms that add or delete info from a database
3. id: identify the form distinctly from other elements on the page

### input
```html
<!--name: each form control needs name attribute-->
<!--size: number of char [old forms: CSS]-->
<form action = "http://www.example.com/login.php" method = "get">
	<p>username:<input type = "text" name = "username" size = "15" maxlength = "30" /></p>
	<p>password:<input type = "password" name = "password" size = "15" maxlength = "30" /></p>
</form>
```

### textarea
```html
<form action = "http://www.example.com/comments.php" method = "get">
	<p>What do you think of this gig</p>
	<textarea name = "comments" cols = "20" rows = "4">Enter your comments</textarea>
</form>
```

### radio btn
```html
<!--checked: which val should be selected when page loads-->
<form action = "http://www.example.com/profile.php">
	<p>Please select your favorite genre</p><br/>
	<input type = "radio" name = "genre" value = "rock" checked = "checked"/> Rock
	<input type = "radio" name = "genre" value = "pop"/> Pop
	<input type = "radio" name = "genre" value = "jazz"/> Jazz
</form>
```

### checkbox
```html
<form action = "http://www.example.com/profile.php">
	<p>Please select your favorite music service(s)</p><br/>
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
		<option value = "iphone" selected = "selected">iPod</option>
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
	<input type = "image" src = "image/subscribe.png" width = "100" height ="20"/>
</form>
```

### button & hidden controls
```html
<!--input hidden: allow page authors to add val to forms users can't see-->
<!--author might use hidden field to indicate which page the user was on when submitting a form-->
<form action = "http://www.example.com/add.php">
	<button><img src = "image/add.gif" alt = "add" width = "10" height = "10"/>Add</button>
	<input type = "hidden" name = "bookmark" value = "lyrics"/>
</form>
```

### labelling form controls
1. wrap around text and form input 
2. separate form and use 'for' to indicate which form to label

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
	<input type = "search" name = "search" placeholder = "Enter keyword"/>
	<input type = "submit" name = "submit"/>
</form>
```

## Extra markup

### The Evolution of HTML
HTML4 XHTML HTML5

### DOCTYPE
Tells a browser which version of HTML the page is using and render page correctly

```html
<!--HTML5-->
<!DOCTYPE html>
<!--HTML4-->
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Traditional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<!--Traditional XHTML 1.0-->
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Traditional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-traditional.dtd">
<!--Strict XHTML 1.0-->
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<!--XML Declaration-->
<?xml version = "1.0" ?>
```

### id
Any HTML elements can carry id attr which uniquely identify themselves. useful in CSS and javascript
```html
<p id = "pullquote">This text appearance can be changed by CSS</p>
```

### class
unlike id attr, elements can share a class attr. If you would like to indicate that an element
<br/>belongs to several classes, you can separate class names with a space. 
<br/>e.g. class="important admittance"

```html
<p class = "important">this is a public announcement...</p>
<p class = "important admittance">Hours: 9-5</p>
```

### Block or inline element
always appear to start on a new line or always appear to continue on the same line

### Grouping text & elements in a block or inline
Group a set of elements together in one block-level box. div element will start on a new line

```html
<!--in a block-->
<div id = "header"><img src = "images/logo.gif" alt = "Anish Kapoor"/></div>
<!--inline-->
<p>Anish Kapoor exhibited at the <span class="gallery">Tate Modern</span>gallery in London</p>
```

### iframe
iframe is like a window that has been cut into your page where you can see another page.
* scrolling (html4 xhtml)
* frameborder (html4 xhtml)
* seamless (html5) for iframe where scrollbars are not desired

```html
<iframe 
	src = "http://maps.google.co.uk/maps?q=moma+new+york&amp;output=embed"
	width="450" height="350" frameborder="0" scrolling="no">
</iframe>
```

### meta
Not visible to users but fulfills a number of purposes such as telling search engines about your page,<br/>who created it, and whether or not it is time sensitive.(expire)

* meta name: property you are setting (e.g. description keywords robots)
* content: value to give to the property
  * robots-noindex: page should not be added
  * robots-nofollow: should be added to search engine results but not any pages that it links to
* meta http-equiv
  * pragma: prevents browser from caching the page
  * expires: indicate when the page should expire(no longer cached)

```html
<head><!--robots indicate whether search engines should add this page to their search results-->
	<meta name="description" content="An Essay on Installation Art"/>
	<meta name="keywords" content="instgallation, art, opinion"/>
	<meta name="robots" content="nofollow"/>
	<meta http-equiv="author" content="Jon Duckett"/>
	<meta http-equiv="pragma" content="no-cache"/>
	<meta http-equiv="expires" content="Fri, 04 Apr 2014 23:59:59 GMT"/>
</head>
```
### Escape char


## Flash Video Audio
1. Flash (.fla exported into .swf) for use on web pages
2. HTML5 video audio tag to add video or audio on web pages
3. YouTube or SoundCloud services

### How Flash works
Exporting .fla to .swf creates code to embed the flash movie in your page.<br/>

### Use of Flash
Fewer websites use Flash since JavaScript lib(script.aculo.us JQuery) made it easy to create animation<br/>
Browsers are switching to HTML5 video audio tags

### Adding a Flash Movie
SWFObject checks if user's browser is capable of playing Flash. <br/>
If it can, scripts will replace div content with .swf
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Adding a Flash Movie</title>
		<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/swfobject/2.2/swfobject.js"></script>
		<script type="text/javascript">
			swfobject.embedSWF("test.swf","myContent", "400","300","10.0.0","expressInstall.swf");
		</script>
	</head>
	<body>
		<div id="myContent">
			<p>My content test</p>
		</div>
	</body>
</html>
```

### Understanding video formats and players
* Flash or HTML5 video can be used
* encode video formats to WebM or MP4 format

### Using hosted video services

### Preparing a flash video for your site
1. convert into FLV format
2. find FLV player to play the video (osflv.com longtailvideo.com)
3. include the player & video in your page, using javascript SWFObject

### Adding a flash video to your pages
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Adding a Flash Video</title>
		<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/swfobject/2.2/swfobject.js"></script>
		<script type="text/javascript">
			var flashvars = {};
			var params = {movie:"video/puppy.flv"};
			swfobject.embedSWF("flash/osplayer.swf","snow", "400","320","8.0.0",flashvars,params);
		</script>
	</head>
	<body>
		<div id="snow">
			<p>A video of a puppy playing in the snow</p>
		</div>
	</body>
</html>
```

### HTML5 : preparing video for your pages
* You need to supply your video in more than one format for multiple browsers.
* H264: Safari IE,  WebM: Android Chrome Firefox Opera 

### HTML5 : adding video to your pages
* preload: tells browser what to do in page loading [none auto metadata]
* controls: browser should apply its own controls for playback
* autoplay: play automatically
* loop: repeat playing

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Adding HTML5 Video</title>
	</head>
	<body>
		<video src="video/puppy.mp4" poster="image/puppy.jpg" width="400" height="300" preload controls loop>
			<p>A video of a puppy playing in the snow</p>
		</video>
	</body>
</html>
```

### Multiple video sources
Use ```<video><source>``` to specify multiple video formats

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Multiple video sources</title>
	</head>
	<body>
		<video poster="image/puppy.jpg" width="400" hiehgt="320" preload controls loop>
		<source src="video/puppy.mp4" type='video/mp4;codecs="avc1.42E01E, mp4a.40.2"'/>
		<source src="video/puppy.webm" type='video/webm;codecs="vp8, vorbis"'/>
		<p>A video of a puppy playing in the snow</p>
	</body>
</html>
```

### HTML5: combining flash & HTML5 video
Ensure users from different browsers. HTML5 further provides playback, adopting different sized screens or<br/>
telling different parts of a page to change when the video reaches a certain point.

### Adding audio to web pages
Similar to video 1. hosted service 2. Flash 3. HTML5 video audio tag

### Adding a flash MP3 player
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Adding a Flash MP3 Player</title>
		<script type="text/javascript"
			src="http://ajax.googleapis.com/ajax/libs/swfobject/2.2/swfobject.js"></script>
		<script type="text/javascript">
			var flashvars={};
			var params={mp3:"audio/test-audio.mp3"};
			swfobject.embedSWF("flash/player_mp3_1.0.0.swf","music-player","200","20","8.0.0",
				flashvars, params);
		</script>
	</head>
	<body>
		<div id="music-player">
			<p>This browser does not support our Flash music player.</p>
		</div>
	</body>
</html>
```

### HTML5: Adding HTML audio to your pages
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Adding HTML5 Audio</title>
	</head>
	<body>
		<audio src="audio/test-audio.ogg" controls autoplay>
			<p>This browser does not support our audio format.</p>
		</audio>
	</body>
</html>
```

### HTML5: Multiple audio sources
provide multiple audio formats for different browsers
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Multiple Audio Sources</title>
	</head>
	<body>
		<audio controls autoplay>
			<source src="audio/test-audio.ogg"/>
			<source src="audio/test-audio.mp3"/>
			<p>This browser does not support our audio format.</p>
		</audio>
	</body>
</html>
```

### Example: both Flash and HTML5 enabled
Ensure users from different browsers
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Flash Video Audio</title>
		<script type="text/javascript"
			src="http://ajax.googleapis.com/ajax/libs/swfobject/2.2/swfobject.js"></script>
		<script type="text/javascript">
			var flashvars={};
			var params={movie:"video/puppy.flv"};
			swfobject.embedSWF("flash/osplayer.swf","snow","400","320","8.0.0",flashvars,params);
		</script>
	</head>
	<body>
		<video poster="image/puppy.jpg" width="400" height="320" controls="controls">
		<source src="video/puppy.mp4" type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'/>
		<source src="video/puppy.webm" type='video/webm; codecs="vp8, vorbis"'/>
		<div id="snow">
			<p>This browser does not support our video formats.</p>
		</div>
	</body>
</html>
```


## CSS
CSS allows you to create rules that control the way that each individual box is presented

1. selector
2. declaration {property: value}

```html
<!--example.html-->
<!DOCTYPE html>
<html>
	<head>
		<title>Introducing CSS</title>
		<link href="css/example.css" type="text/css" rel="stylesheet"/>
	</head>
	<body>
		<h1>From Garden to Plate</h1>
		<p>A <i>potager</i> is a French term for an ornamental vegetable or kitchen garden...</p>
		<h2>What to Plant</h2>
		<p>Planes are chosen as much for their functionality as for their color and form...</p>
	</body>
</html>
```

```css
/*example.css*/
body {
	font-family: Arial, Verdana, sans-serif;
	background-color: rgb(185,179,175);}
h1,h2 {
	color: #ee3e80;}
p {
	color: #665544}
```

### Using internal CSS
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Introducing CSS</title>
		<style type="text/css">
			body {
				font-family: Arial, Verdana, sans-serif;
				background-color: rgb(185,179,175);}
			h1,h2 {
				color: #ee3e80;}
			p {
				color: #665544}
		</style>
	</head>
	<body>
		<h1>From Garden to Plate</h1>
		<p>A <i>potager</i> is a French term fro an ornamental vegetable or kitchen garden...</p>
		<h2>What to Plant</h2>
		<p>Planes are chosen as much for their functionality as for their color and form...</p>
	</body>
</html>
```

### CSS selectors
target rules to specific elements in an HTML document
```html
<!DOCTYPE html>
<html>
	<head>
		<title>CSS selectors</title>
		<link href="css/example.css" type="text/css" rel="stylesheet"/>
	</head>
	<body>
		<h1 id="top">Kitchen Garden Calendar</h1>
		<p id="introduction">Here you can read our handy guide about what to do when</p>
		<h2>Spring</h2>
		<ul>
			<li><a href="mulch.html">Spring mulch vegetable beds</a></li>
			<li><a href="potato.html">Plant out early potatoes</a></li>
			<li><a href="tomato.html">Sow tomato seeds</a></li>
		</ul>
		<p class="note">Contact: <a href="mailto:ivy@example.org">ivy@example.org</a></p>
		<p><a href="#top">Top of page</a></p>
	</body>
</html>
```

<table>
	<tr>
		<th>SELECTOR</th>
		<th>MEANING</th>
		<th>EXAMPLE</th>
	</tr>
	<tr>
		<th>Universal</th>
		<td>Applies to all elements in the document</td>
		<td>* {} <br/>targets all elements on the page</td>
	</tr>
	<tr>
		<th>Type</th>
		<td>Matches element names</td>
		<td>h1,h2,h3{} <br/>targets h1 h2 h3 elements</td>
	</tr>
	<tr>
		<th>Class</th>
		<td>Matches an elements whose class attribute matches one of the values after the period(or full stop) symbol</td>
		<td>.note{} <br/>targets any element whose class attribute has a value of note <br/>p.note{} <br/>targets only &ltp&gt elements whose class attribute has a value of note</td>
	</tr>
	<tr>
		<th>ID</th>
		<td>Matches an elements whose id attribute has a value that matches the one specified afterthe hash symbol</td>
		<td>#introduction {} <br/>targets element whose id has a value of introduction</td>
	</tr>
	<tr>
		<th>Child</th>
		<td>Matches an element that is a direct child of another</td>
		<td>li>a {} <br/>targets any &lta&gt elements that are children of an &ltli&gt elements(but not other &lta&gt elements in the page)</td>
	</tr>
	<tr>
		<th>Descendant</th>
		<td>Matches an element that is a descendent of another specified element(not just a direct child of that element)</td>
		<td>p a {} <br/>targets any &lta&gt elements that sit inside a &ltp&gt elements even if there are other elements nested between them</td>
	</tr>
	<tr>
		<th>Adjacent Sibling</th>
		<td>Matches an element that is the next sibling of another</td>
		<td>hl+p {} <br/>targets the first &ltp&gt element after any &lth1&gt element (but not other &ltp&gt elements)</td>
	</tr>
	<tr>
		<th>General Sibling</th>
		<td>Matches an element that is a sibling of another, although it does not have to be the directly preceding element</td>
		<td>h1~p {} <br/>If you had two &ltp&gt elements that are siblings of an &lth1&gt element, this rule would apply to both</td>
	</tr>
</table>

### How CSS rules cascade
If there are two or more rules that apply to the same element, it is important to understand which will take precedence.

* Last Rule
* Specificity
* Important

```html
<h1>Potatoes</h1>
<p id="intro">There are <i>dozens</i> of different <b>potato</b> varieties.</p>
<p>There are usually described as early, second early and maincrop potatoes.</p>
```

```css
*{font-family: Arial,Verdana,sans-serif;}
h1{font-family: "Courier New", monospace;}
i{color: green}
i{color: red;}
b{color:pink;}
p b{color: blue !important}
p b{color: violet;}
p#intro{font-size: 100%}
p{font-size: 75%;}
```

### Inheritance
body element ```css body{/*css*/}```is inherited by child elements except background color or border properties.<br/>
one can force a lot of properties to inherit values from their parent elements by using inherit.

```html
<div class="page">
	<h1>Potatoes</h1>
	<p>There are dozens of different potato varieties.</p>
	<p>They are usually described as early, second early and maincrop potatoes.</p>
</div>
```

```css
/*div class will inherit body element padding property*/
body{
	font-family: Arial, Verdana, sans-serif;
	color: #665544;
	padding: 10px;
}
.page{
	border: 1px solid #665544;
	background-color: #efefef;
	padding: inherit; /*border property forced to inherit*/
}
```

### Test in multiple browsers and fix bugs
* PositionIsEverything.net
* QuirksMode.org

## Color

### Foreground color
* RGB values (red, green, blue)
* HEX codes
* Color names

```css
h1{
	color: DarkCyan;}
h2{
	color: #ee3e80;}
p{
	color: rgb(100,100,90);}
```

### Background color
```css
body{
	background-color: rgb(200,200,200);}
h1{
	background-color: DarkCyan;}
h2{
	background-color: #ee3e80;}
p{
	background-color: white;}
```

### Understanding color
* RGB value
* HEX code
* Color name
* Hue
* Saturation: amount of gray (%)
* Brightness(Lightness): amount of black (%)
* Contrast

### CSS3: Opacity
use opacity (0.0~1.0) or rgba to specify fourth value, alpha

```css
/*use both RGB and RGBA properties for different browsers*/
p.one{
	background-color: rgb(0,0,0);
	opacity:0.5;
}
p.two{
	background-color: rgb(0,0,0);
	background-color: rgba(0,0,0, 0.5);
}
```

### CSS3: HSL & HSLA
* Hue: colloquial idea of color (0~360 degree)
* Saturation: amount of gray (%)
* Lightness: amount of black (%)
* Alpha: opacity/transparency (0~1.0)

```css
body{
	background-color: #C8C8C8;
	background-color: hsl(0,0%,78%);
}
p{
	background-color: #ffffff;
	background-color: hsla(0,100%,100%,0.5);
}
```


## Text(css)

### Typeface
* serif (Georgia, Times, Times New Roman)
* sans-serif (Arial, Verdana, Helvetica)
* monospace (Courier, Courier New)
* cursive (Comic Sans MS, Monotype Corsiva)
* fantasy (Impact, Haettenschweiler)

### Weight Style stretches
* Weight(light medium bold black)
* Style(normal italic oblique)
* Stretch(condensed regular extended)

### Typeface choices
* font-family: installed
* @font-face: download, license to use the font must permit its distribution using @font-face
* Service-Based Font-Face: paid license
* Images
* SIFR
* Cufon

### Font-Family
### Font-Size

### Units of Type size
* Twelve Pixel Scale (12px == 75% == .75em)
* Sixteen Pixel Scale (16px == 100% == 1em)

### More font choice @font-face
@font-face allows a version of the font to be downloaded to the user's computer.<br/>
It is important that the license for the font permits it to be used in this way.

### Open source or paid fonts
* fontsquirrel.com
* fontex.org
* openfontlibrary.org
* www.google.com/webfonts

charged:
* typekit.com
* kernest.com
* fontspring.com

### Understanding font formats
The various font formats should appear in your code in this order: 1.eot 2.woff 3. ttf/otf 4.svg

```css
@font-face{
	font-family: 'ChuckFiveRegular';
	src: url('fonts/chuckfive.eot');
	src: url('fonts/chuckfive.eot?#iefix') format('embedded-opentype'),
		 url('fonts/chuckfive.woff') format('woff'),
		 url('fonts/chuckfive.ttf') format('truetype'),
		 url('fonts/chuckfive.svg#ChuckFiveRegular') format('svg');
}
```

### Font weight and sytle
```css
.credits{
	font-weight: bold; /*normal;*/
	font-style: italic; /*normal oblique(angled normal)*/
}
```

### Upper LowerCase
```css
h1{text-transform: uppercase;}
h2{text-transform: lowercase;}
h3{text-transform: capitalize;} /*first letter of each word*/
```

### Underline & Strike
```css
.credits{text-decoration: underline;} /*text underline*/
h1{text-decoration: overline;} /*text overline*/
h2{text-decoration: line-through;}
h3{text-decoration: blink;} /*flash animation*/
a{text-decoration: none;} /*remove any applied decoration*/
```

### Line height
```css
p{line-height: 1.4em;} /*line height = leading + font size*/
```

### Letter & Word spacing
```css
.credits{
	text-transform: uppercase;
	font-weight: bold;	
	letter-spacing: .2em;
	word-spacing: 1em;
}
```

### Alignment
```css
/*justify: every line in a paragraph except the last line should be set to take up 
the full width of the containing box */
h1{text-align: left;}
h2{text-align: center;}
h3{text-align: right;}
p{text-align: justify;}

/*used with <img> <em> or <strong>*/
#six-months{vertical-align: text-top;}
#one-year{vertical-align: baseline;}
#two-years{vertical-align: text-bottom;}
/*other values: sub, super, top, middle, bottom*/
```

### Indent
indent the first line of text within an element

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Briard</title>
		<!--<link href="css/example.css" type="text/css" rel="stylesheet"/>-->
		<style type="text/css">
			h1 {
				background-image: url("image/logo(1).gif");
				background-repeat: no-repeat;
				text-indent: -9999px;
				width: 165px;
				height: 100px;}
			.credits {
				text-indent: 20px;}
		</style>
	</head>
	<body>
		<h1>Briards</h1>
		<p class="credits">by anonymous</p>
		<p class="one">The briard is known as a heart wrapped in fur.</p>
		<p class="five">The briard is known as a heart wrapped in fur.</p>
	</body>
</html>
```

```css
h1{
	background-image: url("../image/logo.gif");
	background-repeat: no-repeat;
	text-indent: -9999px;
}
.credits{text-indent: 20px;}
```

### CSS3: Drop Shadow
three lengths and a color for the drop shadow 1. lr 2. tb 3. amount of blur 4. color

```css
p.one{
	background-color: #eeeeee;
	color: #666666;
	text-shadow: 1px 1px 0px #000000;
}
p.five{
	background-color: #aaaaaa;
	color: #ffffff;
	text-shadow: -1px -1px #666666;
}
```

### First letter or line
specify different value for the first letter or line of text inside pseudo-elements 

```css
p.intro:first-letter{font-size: 200%;}
p.intro:first-line{font-weight: bold;}
```

### Styling Links
```css
a:link{color: deeppink; text-decoration: none;}
a:visited{color: black;}
a:hover{color: deeppink;text-decoration: underline;}
a:active{color: darkcyan;}
```

### Responding to users
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Hover Active Focus</title>
		<style type="text/css">
			input {
				padding: 6px 12px 6px 12px;
				border: 1px solid #665544;
				color: #ffffff;}
			input.submit:hover {
				background-color: #665544;}
			input.submit:active {
				background-color: chocolate;}
			input.text {
				color: #cccccc;}
			input.text:focus {
				color:#665544;}
		</style>
	</head>
	<body>
		<form>
			<input type="text" class="text" value="Enter email address...">
			<input type="submit" class="submit">
		</form>
	</body>
</html>
```

### Attribute selectors
set of attribute selectors that allow you to create rules that apply to elements that<br/>
have an attribute with a specific value.

<table>
	<tr>
		<th>SELECTOR</th>
		<th>MEANING</th>
		<th>EXAMPLE</th>
	</tr>
	<tr>
		<th>EXISTENCE</th>
		<td>[]<br/>Matches a specific attribute (whatever its value)</td>
		<td>p[class]<br/>Targets any &ltp&gt element with an attribute called class</td>
	</tr>
	<tr>
		<th>EQUALITY</th>
		<td>[=]<br/>Matches a specific attribute with a specific value</td>
		<td>p[class="dog"]<br/>Targets any &ltp&gt element with an attribute called class whose value is dog</td>
	</tr>
	<tr>
		<th>SPACE</th>
		<td>[~=]<br/>Matches a specific attr whose value appears in a space-separated list of words</td>
		<td>p[class~="dog"]<br/>Targets any &ltp&gt element with an attr called class whose value is a list of space-separated words, one of which is dog</td>
	</tr>
	<tr>
		<th>PREFIX</th>
		<td>[^=]<br/>Matches a specific attr whose value begins with a specific string</td>
		<td>p[attr^="d"]<br/>Targets any &ltp&gt element with an attr whose value begins with the letter "d"</td>
	</tr>
	<tr>
		<th>SUBSTRING</th>
		<td>[*=]<br/>Mathces a specific attr whose value contains a specific substring</td>
		<td>p[attr*="do"]<br/>Targets any &ltp&gt element with an attr whose value contains the letter "do"</td>
	</tr>
	<tr>
		<th>SUFFIX</th>
		<td>[$=]<br/>Matches a specific attr whose value ends with a specific string</td>
		<td>p[attr$="g"]<br/>Targets any &ltp&gt element with an attr whose value ends with the letter "g"</td>
	</tr>
</table>

### Example

## Boxes
