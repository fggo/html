* [Structure](#structure)
* [Text](#text)
* [Semantic Markup](#semantic-markup)
* [Lists](#lists)
* [Links](#links)
* [Images](#images)
* [Table](#table)
* [Forms](#forms)
* [Extra markup](#extra-markup)
* [Flash Video Audio](#flash-video-audio)
* [CSS](#css)
* [Color](#color)
* [Text](#textcss)
* [Boxes](#boxes)
* [Lists, Tables and Forms](#list-table-and-form)
* [Layout](#layout)
* [Images](#images)
* [HTML5 Layout](#html5-layout)
* [Process and Design](#process-and-design)
* [Practical Information](#practical-information)

# Structure
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

# Text
```html
<!--Bold Italic-->
<b>bold</b>
<i>italic</i>

<!--Superscript Subscript-->
E = MC<sup>2</sup>
H<sub>2</sub>O

<!--White space: two or more spaces collapse to one-->
<p>Hello     World</p>

<!--Line Breaks-->
Line One<br/>Line Two<br/>

<!--Horizontal rules-->
<p>Current Topic</p>
<hr/>
```

# Semantic markup
- Text elements that are not intended to affect the structure of web pages

```html
<!--Strong-->
<strong>Warning!</strong> This is a tiger cage.

<!--Emphasis that subtly changes the meaning of a sentence-->
<p><em>I</em> think water is empty</p>
<p>I <em>think</em> water is empty</p>
<p>I think water is <em>empty</em></p>

<!--Block quote-->
<blockquote cite = "https://en.wikipedia.org/wiki/Floyd_Mayweather_Jr.">
	<p>TMT</p>
</blockquote>

<!--Quotation mark-->
<q>Fly like a butterfly. Sting like a bee.</q>

<!--Abbreviation-->
<abbr title = "Professor">Prof</abbr> will discuss the topic.

<!--Acronym-->
<acronym title = "President Of The United States">POTUS</acronym> is flying.

<!--Citation-->
<cite>A Brief History of Time</cite> by Stephen Hawking has sold over ten million copies.

<!--Definitions-->
<dfn>Black hole</dfn> is a region of space from which nothing, not even light, can escape.

<!--Author details: Address contains contact details-->
<address>
	<p><a href = "mailto:homer@example.org"> homer@example.org</a> </p>
	<p>742 Evergreen Terrace, Springfield.</p>
</address>

<!--Changes to content-->
<del>worst</del> <ins>best</ins> season.

<!--No longer relevant-->
<s>Price is $200</s><br/>
   Now Price is $150
```

# Lists

```html
<!--Ordered Lists-->
<ol>
	<li>Buy Kaby Lake CPU</li>
	<li>Buy 512GB SSD</li>
	<li>Buy U2414H monitor</li>
</ol>

<!--Unordered Lists-->
<ul>
	<li>melon</li>
	<li>water</li>
	<li>egg</li>
	<li>beef</li>
</ul>

<!--Definition Lists-->
<dl>
	<dt>Bread</dt>
	<dd>Bread is a staple food prepared from a dough of flour and water.</dd>

	<dt>Coffee</dt>
	<dd>Coffee is a brewed drink prepared from roasted coffee beans.</dd>
</dl>

<!--Nested Lists-->
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

# Links

## Absolute and Relative URL
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

## Directory structure
main homepage index.html; examplearts.com returns examplearts.com/index.html

## Relative URL
```html
<a href = "reviews.html">Reviews</a>
<a href = "music/listings.html">Listings</a>
<a href = "movies/dvd/reviews.html">Reviews</a>
<a href = "../index.html">Home</a>
<a href = "../../index.html">Home</a>
```

```html
<!--Email Links-->
<a href = "mailto:jon@example.org">Email Jon</a>

<!--Links in new window-->
<a href = "https://www.youtube.com/" target = "_blank">Youtube</a>

<!--Link to same page-->
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

<!--Link to different page-->
absolute or relative URL, followed by the value of the id attr
<a href = "http:/www.htmlandcssbookcom/#bottom">book</a>
```

# Images
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

## img align [old code]
```html
'align' attr is no longer used in HTML5. Use CSS to control alignment of images
<!--left, right, top, middle, bottom (first line)-->
<p>
	<img
	src = "work.jpg" alt ="stretches before workout" title = "work" height = "100" width = "150"
	align = "left">Working out is essential for people who works on the desk daily.
</p>
```

## Rules for creating img
1. img in right format (jpeg gif png)
2. img in right size
3. img in correct resolution (72 px)

## Tools to edit img
1. Adobe Photoshop
2. GIMP
4. Blender
5. Abobe Fireworks
6. Pixelmator
7. PaintShop Pro
8. Paint.net

## Bitmap: jpeg gif png
* .jpeg for img with many different colors
* .gif .png for img with few colors or large areas of the same color

# img dimension
reduce, increase, change shapes of an image

## img resolution
image for web should have a resolution of 72 ppi

## Vector img
Differs from bitmap image and resolution-independent, commonly created with Adobe Illustrator. Place points on a gird and draw lines between them and color can be fill in

## Animated gifs
Shows several frames of an image in sequence to create simple animations. Due to increasing file sizes, gif is only suitable for simple illustration

## Transparency
Creating a partially transparent image for web involves selecting one of two formats :
* transparent gif : straight edged img
* png : diagonal, round, semi-opaque, drop-shadow img


## figure figcaption
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

# Table

## table heading
```html
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
```

## spanning columns
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

## spanning rows
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

## thead tbody tfoot
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

## Table Width & Spacing [old code]
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

## Table Border & Background [old code]
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

# Forms

## Form control

## adding text
1. text input
2. pw input
3. text area

## making choices
1. radio btn
2. checkboxes
3. drop-down boxes

## how forms work
1. user fills in a form and press submit btn
2. (name, value) pair of each form control is sent to the server
3. server processes info using lang like PHP, C#, VB.net, Java and stores info in a database.
4. server creates a new page to send back to the brower based on the info received

## form structure
1. action: url for the page on the server receiving submitted info
2. method : [get, post]
  * get: short forms(e.g. search boxes) to get data from web server
  * get: does not send info that should be added to or deleted from database
  * post: long forms to upload a file, might contain sensitive data (pw)
  * post: forms that add or delete info from a database
3. id: identify the form distinctly from other elements on the page

## input
```html
<!--name: server needs to know which form control each data was entered into-->
<!--size: number of char [old forms; now controlled in CSS]-->
<form action = "http://www.example.com/login.php" method = "get">
	<p>username:<input type = "text" name = "username" size = "15" maxlength = "30" /></p>
	<p>password:<input type = "password" name = "password" size = "15" maxlength = "30" /></p>
</form>
```

## textarea
```html
<form action = "http://www.example.com/comments.php" method = "get">
	<p>What do you think of this gig</p>
	<textarea name = "comments" cols = "20" rows = "4">Enter your comments</textarea>
</form>
```

## radio btn
```html
<!--checked: which val should be selected when page loads-->
<form action = "http://www.example.com/profile.php">
	<p>Please select your favorite genre</p><br/>
	<input type = "radio" name = "genre" value = "rock" checked = "checked"/> Rock
	<input type = "radio" name = "genre" value = "pop"/> Pop
	<input type = "radio" name = "genre" value = "jazz"/> Jazz
</form>
```

## checkbox
```html
<form action = "http://www.example.com/profile.php">
	<p>Please select your favorite music service(s)</p><br/>
	<input type = "checkbox" name = "service" value = "itunes" checked = "checked"/> iTunes
	<input type = "checkbox" name = "service" value = "lastfm"/> Last.fm
	<input type = "checkbox" name = "service" value = "spotify"/> Spotify
</form>
```

## dropdown list box
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

## multiple select box
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

## file input box
```html
<form action = "http://www.example.com/upload.php" method = "post">
	<p>upload your song in mp3 format</p>
	<input type = "file" name = "user-song"/> <br />
	<input type = "submit" value = "Upload"/>
</form>
```

## submit btn
```html
<!--value: text that appears on the page-->
<form action = "http://www.example.com/subscribe.php">
	<p>subscribe to our email list:</p>
	<input type = "text" name = "email"/>
	<input type = "submit" name = "subscribe" value = "Subscribe"/>
</form>
```

## image btn
```html
<!--alt works as used in <img>-->
<form action = "http://www.example.com/subscribe.php">
	<p>subscribe to our email list:</p>
	<input type = "text" name = "email"/>
	<input type = "image" src = "images/subscribe.png" width = "100" height ="20"/>
</form>
```

## button & hidden controls
```html
<!--input hidden: allow page authors to add val to forms users can't see-->
<!--author might use hidden field to indicate which page the user was on when submitting a form-->
<form action = "http://www.example.com/add.php">
	<button><img src = "images/add.gif" alt = "add" width = "10" height = "10"/>Add</button>
	<input type = "hidden" name = "bookmark" value = "lyrics"/>
</form>
```

## labelling form controls
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

## Grouping form elements
```html
<fieldset>
	<legend>Contact details</legend>
	<label>Email:<br/><input type = "text" name = "email"/></label>
	<label>Mobile:<br/><input type = "text" name = "mobile"/></label>
	<label>Tel:<br/><input type = "text" name = "tel"/></label>
</fieldset>
```

## HTML5: form validation
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

## HTML5: date input
```html
<form action = "http://www.example.com/bookings/" method = "post">
	<label for = "username">Departure date:</label>
	<input type = "date" name = "depart"/>
	<input type = "submit" value = "Submit"/>
</form>
```

## HTML5: email & url input
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

## HTML5: search input
```html
<form action = "http://www.example.org/search.php">
	<p>Search:</p>
	<input type = "search" name = "search" placeholder = "Enter keyword"/>
	<input type = "submit" name = "submit"/>
</form>
```

# Extra markup

## The Evolution of HTML
HTML4 XHTML HTML5

## DOCTYPE
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

## id
Any HTML elements can carry id attr which uniquely identify themselves. useful in CSS and javascript
```html
<p id = "pullquote">This text appearance can be changed by CSS</p>
```

## class
elements can share a single or multiple classes.
```html
<p class = "important">this is a public announcement...</p>
<p class = "important admittance">Hours: 9-5</p> <!--element can share multiple classes-->
```

## Block or inline element
always appear to start on a new line or always appear to continue on the same line

## Grouping text & elements in a block or inline
```html
<!--in a block; div element will start in a new line-->
<div id = "header">
	<img src = "images/logo.gif" alt = "Anish Kapoor"/>
</div>
<!--inline-->
<p>Anish Kapoor exhibited at the <span class="gallery">Tate Modern</span>gallery in London</p>
```

## iframe
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

## meta
Not visible to users but fulfills a number of purposes such as telling search engines about your page, who created it, and whether or not it is time sensitive.(expire)

* name: property you are setting
  - description: to show site description by search engines
  - keywords: separated by comma, no effect in indexing search
  - robots: indicates whether search engines should add this page to their search result or not
  - robots (noindex): page should not be added
  - robots (nofollow): should be added to search engine results but not any pages that it links to
* content: pairs with http-equiv
* http-equiv
  - author: defines author of the page
  - pragma: prevents browser from caching the page
  - expires: indicate when the page should expire(no longer cached)

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

## Escape char

# Flash Video Audio
1. Flash (.fla exported into .swf) for use on web pages
2. HTML5 video audio tag to add video or audio on web pages
3. YouTube or SoundCloud services

## How Flash works
Exporting .fla to .swf creates code to embed the flash movie in your page.

## Use of Flash
Fewer websites use Flash since JavaScript lib(script.aculo.us JQuery) made it easy to create animation. Browsers are switching to HTML5 video audio tags

## Adding a Flash Movie
SWFObject checks if user's browser is capable of playing Flash. If it can, scripts will replace div content with .swf.
```html
<!DOCTYPE html>
<html>
<head>
	<title>Adding a Flash Movie</title>
	<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/swfobject/2.2/swfobject.js"></script>
	<script type="text/javascript">swfobject.embedSWF("flash/bird.swf", "bird", "400", "300", "8.0.0");</script>
	<style type="text/css" media="screen">#bird {visibility:hidden}</style>
</head>
<body>
	<object id="bird" type="application/x-shockwave-flash" data="flash/bird.swf" style="visibility: visible;" height="300" width="400"></object>
</body>
</html>
```

## Understanding video formats and players
* Flash or HTML5 video can be used
* encode video formats to WebM or MP4 format

## Using hosted video services

## Preparing a flash video for your site
1. convert into FLV format
2. find FLV player to play the video (osflv.com longtailvideo.com)
3. include the player & video in your page, using javascript SWFObject

## Adding a flash video to your pages
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

## HTML5 : preparing video for your pages
* You need to supply your video in more than one format for multiple browsers.
* H264: Safari IE,  WebM: Android Chrome Firefox Opera

## HTML5 : adding video to your pages
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
		<video src="video/puppy.mp4" poster="images/puppy.jpg" width="400" height="300" preload controls loop>
			<p>A video of a puppy playing in the snow</p>
		</video>
	</body>
</html>
```

## Multiple video sources
Specify more than one video formats for different kinds of browsers.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Multiple video sources</title>
	</head>
	<body>
		<video poster="images/puppy.jpg" width="400" hiehgt="320" preload controls loop>
			<source src="video/puppy.mp4" type='video/mp4;codecs="avc1.42E01E, mp4a.40.2"'/>
			<source src="video/puppy.webm" type='video/webm;codecs="vp8, vorbis"'/>
			<p>A video of a puppy playing in the snow</p>
		</video>
	</body>
</html>
```

## HTML5: combining flash & HTML5 video
Ensure users from different browsers. HTML5 further provides playback, adopting different sized screens or telling different parts of a page to change when the video reaches a certain point.

## Adding audio to web pages
Similar to video 1. hosted service 2. Flash 3. HTML5 video audio tag

## Adding a flash MP3 player
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

## HTML5: Adding HTML audio to your pages
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

## HTML5: Multiple audio sources
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

## Example: both Flash and HTML5 enabled
Ensure users from different browsers
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Flash, Video and Audio</title>
		<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/swfobject/2.2/swfobject.js"></script>
		<script type="text/javascript">
			var flashvars = {};
			var params = {movie: "../video/puppy.flv"};
			swfobject.embedSWF("flash/osplayer.swf", "snow", "400", "320", "8.0.0", flashvars, params);
		</script>
		<style type="text/css" media="screen">#snow {visibility:hidden}</style>
	</head>
	<body>
		<video poster="images/puppy.jpg" width="400" height="320" controls="controls">
			<source src="video/puppy.mp4" type="video/mp4;codecs=&quot;avc1.42E01E, mp4a.40.2&quot;"/>
			<source src="video/puppy.webm" type="video/webm;codecs=&quot;vp8, vorbis&quot;"/>
			<div id="snow">
				<p>You cannot see this video of a puppy playing in the snow because this browser
				does not support our video formats.</p>
			</div>
		</video>
	</body>
</html>
```

# CSS
CSS allows you to create rules that control the way that each individual box is presented

1. selector
2. declaration {property: value}

## Using external CSS
```html
<!--example.html-->
<!DOCTYPE html>
<html>
	<head>
		<title>Using External CSS</title>
		<link href="css/example.css" type="text/css" rel="stylesheet"/>
	</head>
	<body>
	</body>
</html>
```

```css
/*example.css*/
body {font-family: Arial, Verdana, sans-serif;
	background-color: rgb(185,179,175);}
h1,h2 {
	color: #ee3e80;}
p {
	color: #665544}
```

## Using internal CSS
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Using Internal CSS</title>
		<style type="text/css">
			body {font-family: Arial, Verdana, sans-serif;
				background-color: rgb(185,179,175);}
			h1,h2 {color: #ee3e80;}
			p {color: #665544}
		</style>
	</head>
	<body>
	</body>
</html>
```

## CSS selectors
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
		<td>Matches an elements whose id attribute has a value that matches the one specified after the hash symbol</td>
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
		<td>h1+p {} <br/>targets the first &ltp&gt element after any &lth1&gt element (but not other &ltp&gt elements)</td>
	</tr>
	<tr>
		<th>General Sibling</th>
		<td>Matches an element that is a sibling of another, although it does not have to be the directly preceding element</td>
		<td>h1~p {} <br/>If you had two &ltp&gt elements that are siblings of an &lth1&gt element, this rule would apply to both</td>
	</tr>
</table>

## How CSS rules cascade
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

## Inheritance
body{} is inherited by child elements except background-color or border properties. Use 'inherit' to force properties to inherit values from their parent elements  
```html
<div class="page">
	<h1>Potatoes</h1>
	<p>There are dozens of different potato varieties.</p>
</div>
```

```css
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

## Test in multiple browsers and fix bugs
* PositionIsEverything.net
* QuirksMode.org

# Color

## Foreground color
* RGB values (red, green, blue)
* HEX codes
* Color names

```css
h1{color: DarkCyan;}
h2{color: #ee3e80;}
p{color: rgb(100,100,90);}
```

## Background color
```css
body{background-color: rgb(200,200,200);}
h1{background-color: DarkCyan;}
h2{background-color: #ee3e80;}
p{background-color: white;}
```

## Understanding color
* RGB value
* HEX codec
* Color name
* Hue
* Saturation: amount of gray (%)
* Brightness(Lightness): amount of black (%)
* Contrast

## CSS3: Opacity
use opacity (0.0~1.0) or rgba to specify fourth value, alpha

```css
/*use both RGB and RGBA properties for different browsers*/
p.one{
	background-color: rgb(0,0,0);
	opacity:0.5;}
p.two{
	background-color: rgb(0,0,0);
	background-color: rgba(0,0,0, 0.5);}
```

## CSS3: HSL & HSLA
* Hue: colloquial idea of color (0~360 degree)
* Saturation: amount of gray (%)
* Lightness: amount of black (%)
* Alpha: opacity/transparency (0~1.0)

```css
body{
	background-color: #C8C8C8;
	background-color: hsl(0,0%,78%);}
p{
	background-color: #ffffff;
	background-color: hsla(0,100%,100%,0.5);}
```

# Text(css)

## Typeface
* serif (Georgia, Times, Times New Roman)
* sans-serif (Arial, Verdana, Helvetica)
* monospace (Courier, Courier New)
* cursive (Comic Sans MS, Monotype Corsiva)
* fantasy (Impact, Haettenschweiler)

## Weight, Style, Stretch
* Weight(light medium bold black)
* Style(normal italic oblique)
* Stretch(condensed regular extended)

## Typeface choices
* font-family: installed
* @font-face: download, license to use the font must permit its distribution using @font-face
* Service-Based Font-Face: paid license
* Images
* SIFR
* Cufon

## Font-Family, Font-Size

## Units of Type size
* Twelve Pixel Scale (12px == 75% == .75em)
* Sixteen Pixel Scale (16px == 100% == 1em)

## More font choice @font-face
@font-face allows a version of the font to be downloaded to the user's computer. It is important that the license for the font permits it to be used in this way.

## Open source or paid fonts
* fontsquirrel.com
* fontex.org
* openfontlibrary.org
* www.google.com/webfonts

charged:
* typekit.com
* kernest.com
* fontspring.com

## Understanding font formats
font formats should appear in your code in this order: 1.eot 2.woff 3. ttf/otf 4.svg

```css
@font-face{
	font-family: 'ChuckFiveRegular';
	src: url('fonts/chuckfive.eot');
	src: url('fonts/chuckfive.eot?#iefix') format('embedded-opentype'),
		 url('fonts/chuckfive.woff') format('woff'),
		 url('fonts/chuckfive.ttf') format('truetype'),
		 url('fonts/chuckfive.svg#ChuckFiveRegular') format('svg');}
```

## Font weight, Font sytle
```css
.credits{
	font-weight: bold; /*normal;*/
	font-style: italic; /*normal oblique(angled normal)*/
}
```

## Upper LowerCase
```css
h1{text-transform: uppercase;}
h2{text-transform: lowercase;}
h3{text-transform: capitalize;} /*first letter of each word*/
```

## Underline & Strike
```css
.credits{text-decoration: underline;} /*text underline*/
h1{text-decoration: overline;} /*text overline*/
h2{text-decoration: line-through;}
h3{text-decoration: blink;} /*flash animation*/
a{text-decoration: none;} /*remove any applied decoration*/
```

## Line Height
```css
p{line-height: 1.4em;} /*line height = leading + font size*/
```

## Letter & Word spacing
```css
.credits{
	text-transform: uppercase;
	font-weight: bold;
	letter-spacing: .2em;
	word-spacing: 1em;
}
```

## Alignment
```css
/*justify: every line in a paragraph except the last line should be set to take up
the full width of the containing box */
h1{text-align: left;}
h2{text-align: center;}
h3{text-align: right;}
p{text-align: justify;}
```

```html
<!--Vertical Alignment is used with inline elements like <img> <em> <strong>
values it can take: sub, super, top, middle, bottom-->
<html><head>
		<title>Vertical Align</title>
		<style type="text/css">
			#six-months {vertical-align: text-top;}
			#one-year {vertical-align: baseline;}
			#two-years {vertical-align: text-bottom;}
		</style>
	</head>
	<body>
		<h1>Briard Life Stages</h1>
		<p><img src="images/6-month.gif" width="50" height="50" alt="6 months" id="6-month">6-month</p>
		<p><img src="images/1-year.gif" width="50" height="50" alt="1 year" id="1-year">1-year</p>
		<p><img src="images/2-year.gif" width="50" height="50" alt="2 years" id="2-year">2-year</p>
</body></html>
```

## Indent
indent the first line of text within an element

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Briard</title>
		<!--<link href="css/example.css" type="text/css" rel="stylesheet"/>-->
		<style type="text/css">
			h1 {
				background-image: url("images/logo.gif");
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
		<p class="credits">by Ivy Duckett</p>
	</body>
</html>
```

## CSS3: Drop Shadow
text-shadow: h-shadow v-shadow blur-radius color|none|initial|inherit;

```css
* {	/* offset-x | offset-y | blur-radius | color */
	text-shadow: 1px 1px 2px black;

	/* color | offset-x | offset-y | blur-radius */
	text-shadow: #CCC 1px 0 10px;

	/* offset-x | offset-y | color */
	text-shadow: 5px 5px #558ABB;

	/* color | offset-x | offset-y */
	text-shadow: white 2px 5px;

	/* offset-x | offset-y
	/* Use defaults for color and blur-radius */
	text-shadow: 5px 10px;

	/* Global values */
	text-shadow: inherit;
	text-shadow: initial;
	text-shadow: unset;

	background-color: #eeeeee;
	color: #666666;}
```

## First letter or First line
specify different value for the first letter or line of text inside pseudo-elements

```css
p.intro:first-letter{font-size: 200%;}
p.intro:first-line{font-weight: bold;}
```

## Styling Links
```css
a:link{color: deeppink; text-decoration: none;}
a:visited{color: black;}
a:hover{color: deeppink;text-decoration: underline;}
a:active{color: darkcyan;}
```

## Responding to users
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

## Attribute selectors
set of attribute selectors that allow you to create rules that apply to elements that have an attribute with a specific value.

<table>
	<tr>
		<th>SELECTOR</th>
		<th>MEANING</th>
		<th>EXAMPLE</th>
	</tr>
	<tr>
		<th>EXISTENCE</th>
		<td>[]<br/>Matches a specific attribute (whatever its value)</td>
		<td>p[class]<br/>Targets any &ltp&gt element with an attribute called class<br/>
		span[lang]<br/> Targets any &ltspan&gt element with an attribute called lang</td>
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

## Example
```html
<html>
	<head>
		<title>Text</title>
		<style type="text/css">
			body {
				padding: 20px;}
			h1, h2, h3, a {
				font-weight: normal;
				color: #0088dd;
				margin: 0px;}
			h1 {
				font-family: Georgia, Times, serif;
				font-size: 250%;
				text-shadow: 2px 2px 3px #666666;
				padding-bottom: 10px;}
			h2 {
				font-family: "Gill Sans", Arial, sans-serif;
				font-size: 90%;
				text-transform: uppercase;
				letter-spacing: 0.2em;}
			h3 {
				font-size: 150%;}
			p {
				font-family: Arial, Verdana, sans-serif;
				line-height: 1.4em;
				color: #665544;}
			p.intro:first-line {
				font-weight: bold;}
			.credits {
				font-style: italic;
				text-align: right;}
			a {
				text-decoration: none;}
			a:hover {
				text-decoration: underline;}
		</style>
	</head>
	<body>
		<h1>Briards</h1>
		<h2>A Heart wrapped in fur</h2>
		<p class="intro">The <a class="breed" href="http://en.wikipedia.org/wikiBriard">briard</a>, or berger de brie, is a large breed of dog traditionally used as a herder and guardian of sheep.</p>
		<h3>Breed History</h3>
		<p>The briard, which is believed to have originated in France, has been bred for centuries to herd and to protect sheep. The breed was used by the French Army as sentries, messengers and to search for wounded soldiers because of its fine sense of hearing. Briards were used in the First World War almost to the point of extinction. Currently the population of briards is slowly recovering. Charlemagne, Napoleon, Thomas Jefferson and Lafayette all owned briards.</p>
		<p class="credits">by Ivy Duckett</p>
	</body>
</html>
```

# Boxes

## width Height
```html
<html>
	<head>
		<title>Width Height</title>
		<style type="text/css">
			body {
				font-family: Arial, Verdana, sans-serif;
				color: #111111;}
			div.box{
				height:300px;
				width:300px;
				background-color: #ee3e80;}
			p{
				height:75%;
				width:75%;
				background-color: #e1ddda;}
		</style>
	</head>
	<body>
		<div class="box"><p>The Moog company pioneered the commercial manufacturing</p></div>
	</body>
</html>
```

## Limiting width and height
```css
/*width*/
body {
	font-family: Arial, Verdana, sans-serif;
	color: #111111;}
th {
	border-bottom: 1px solid #0088dd;
	text-align: left;
	color: #0088dd;
	font-weight: normal;}
td {
	min-width: 150px;
	min-height: 200px;
	vertical-align: top;
	line-height: 1.4em;}
td.description {
	min-width: 450px;
	max-width: 650px;
	text-align: left;
	padding: 5px;
	margin: 0px;}
```

```css
/*height (oveflow handling required)*/
body {
	font-family: Arial, Verdana, sans-serif;
	color: #111111;}
h2, p {
	width: 400px;
	font-size: 90%;
	line-height: 1.2em;}
h2 {
	color: #0088dd;
	border-bottom: 1px solid #0088dd;}
p {
	min-height: 10px;
	max-height: 70px;}
```

## Overflowing content
```css
body {
	font-family: Arial, Verdana, sans-serif;
	color: #111111;
	font-size: 90%;
	line-height: 1.2em;
	width: 200px;}
h2 {
	color: #0088dd;
	border-bottom: 1px solid #0088dd;}
p {
	min-height: 30px;
	max-height: 85px;}
p.one {
	overflow: hidden;}
p.two {
	overflow: scroll;}
```

## Border Margin Padding
margin is a gap between borders of two adjacent boxes. <br/>
padding is the space between border and its content inside.

## White space & Vertical margin
use padding & margin

## Border Width
```css
p.one{border-width:2px;}
p.two{border-width:thick;} /*thin medium thick*/
p.three{border-width:1px 4px 12px 4px;} /*top right bottom left*/
```

## Border Style
```css
body {
	font-family: Arial, Verdana, sans-serif;
	color: #111111;}
p {
	width: 250px;
	border-width: 3px;}
p.one {border-style: solid;}
p.two {border-style: dotted;}
p.three {border-style: dashed;}
p.four {border-style: double;}
p.five {border-style: groove;}
p.six {border-style: ridge;}
p.seven {border-style: inset;}
p.eight {border-style: outset;}
```

## Border Color
```css
body {
	font-family: Arial, Verdana, sans-serif;
	color: #111111;}
p {
	border-style: solid;
	border-width: 3px;
	width: 200px;}
p.one {
	border-color: #0088dd;}
p.two {
	border-color: #bbbbaa #111111 #ee3e80 #0088dd;}
```

## Border (in shorthand)
```css
body {
	font-family: Arial, Verdana, sans-serif;
	color: #111111;}
p {
	width: 250px;
	border: 3px dotted #0088dd;}
```

## Padding
space between the content of an element and its border

```css
p{
	width:275px;
	border: 2px solid #0088dd;}
p.example{
	padding:10px;}
/*padding-top right bottom left or
padding: 10px 5px 3px 1px;*/
```

## Margin
gap between boxes

```css
p{
	width:275px;
	border: 2px solid #0088dd;}
p.example{
	margin:20px;}
/*margin-top right bottom left or
margin: 10px 5px 3px 1px;*/
```

## Centering Content
set the following properties:

1. width of the box
2. margin left and right as 'auto'

[old browser]
- text-align: center for the element that the box sits inside (inherited by child elements)

```css
body{
	text-align:center;}
p{
	width:300px;
	padding:50px;
	border: 20px solid #0088dd;}
p.example{
	margin: 10px auto 10px auto;
	text-align:left;}
```

## Change Inline/Block
'inline-block' causes a block-level element to flow like an inline element, while retaining other features of a block-level element.
```css
li{display:inline;  /*display: inline  block  inline-block  none*/
	margin-right:10px;}
li.coming-soon{display:none;}
```

## Hiding boxes
hide but unlike display:none; it leaves a space where the element would have been.

```css
li{display:inline;
	margin-right:10px;}
li.comming-soon{visibility:hidden;} /*visiblity: visible*/
```

## CSS3: Border Images
```html
<html><head>
		<title>Border Image</title>
		<style type="text/css">
			p {
				width: 197px;
				height: 54px;
				border: 11px solid #ffffff;}
			p.one {
				-moz-border-image: url("images/dots.gif") 11 11 11 11 stretch;
				-webkit-border-image: url("images/dots.gif") 11 11 11 11 stretch;
				border-image: url("images/dots.gif") 11 11 11 11 stretch;}
			p.two {
				-moz-border-image: url("images/dots.gif") 11 11 11 11 round;
				-webkit-border-image: url("images/dots.gif") 11 11 11 11 round;
				border-image: url("images/dots.gif") 11 11 11 11 round;}
		</style>
	</head>
	<body>
		<p class="one"></p>
		<p class="two"></p>
</body></html>
```

## CSS3: Box Shadows
Horizontal, Vertical Offeset, Blur distance, Spread of shadow. First two & color should me specified.

```css
p {
	width: 100px;
	height: 100px;
	background-color: #e1ddda;
	margin: 20px;
	display: inline-block;}
p.one {
	-moz-box-shadow: -5px -5px #777777;
	-webkit-box-shadow: -5px -5px #777777;
	box-shadow: -5px -5px #777777;} /*horizontal (negative left) and vertical(negative top)*/
p.two {
	-moz-box-shadow: 5px 5px 5px #777777;
	-webkit-box-shadow: 5px 5px 5px #777777;
	box-shadow: 5px 5px 5px #777777;}  
p.three {
	-moz-box-shadow: 5px 5px 5px 5px #777777;
	-webkit-box-shadow: 5px 5px 5px 5px #777777;
	box-shadow: 5px 5px 5px 5px #777777;} /*spread of shadow in all directions*/
p.four {
	-moz-box-shadow: 0 0 10px #777777;
	-webkit-box-shadow: 0 0 10px #777777;
	box-shadow: 0 0 10px #777777;}
p.five {
	-moz-box-shadow: inset 0 0 10px #777777;
	-webkit-box-shadow: inset 0 0 10px #777777;
	box-shadow: inset 0 0 10px #777777;} /*inset: inner shadow*/
```

## CSS3: Rounded Corners
```css
p {
	border: 5px solid #ee3e80;
	padding: 20px;
	width: 275px;
	border-radius: 10px;
	-moz-border-radius: 10px;
	-webkit-border-radius: 10px;}
```

## CSS3: Elliptical Shapes
specify horizontal and vertical parts of the rounded corners

```css
p {
	border: 5px solid #ee3e80;
	padding: 10px;
	width: 100px;
	height: 100px;
	display: inline-block;
	margin: 20px;}
p.one {
	border-top-left-radius: 80px 50px;
	-moz-border-radius-top-left: 80px 50px;
	-webkit-border-radius-top-left: 80px 50px;}
p.two {
	border-radius: 1em 4em 1em 4em / 2em 1em 2em 1em;
	-moz-border-radius: 1em 4em 1em 4em / 2em 1em 2em 1em;
	-webkit-border-radius:  1em 4em 1em 4em / 2em 1em 2em 1em;}
p.three {
	padding: 0px;
	border-radius: 100px;
	-moz-border-radius: 100px;
	-webkit-border-radius: 100px;}
```

## Example
```html
<html><head>
		<title>Boxes</title>
		<style type="text/css">
			body {
				font-size: 80%;
				font-family: "Courier New", Courier, monospace;
				letter-spacing: 0.15em;
				background-color: #efefef;}
			#page {
				max-width: 940px;
				min-width: 720px;
				margin: 10px auto 10px auto;
				padding: 20px;
				border: 4px double #000;
				background-color: #ffffff;}
			#logo {
				width: 350px;
				margin: 10px auto 25px auto;}
			ul {
				width: 570px;
				padding: 15px;
				margin: 0px auto 0px auto;
				border-top: 2px solid #000;
				border-bottom: 1px solid #000;
				text-align: center;}
			li {
				display: inline;
				margin: 0px 3px;}
			p {
				text-align: center;
				width: 600px;
				margin: 20px auto 20px auto;
				font-weight: normal;}
			a {
				color: #000000;
				text-transform: uppercase;
				text-decoration: none;
				padding: 6px 18px 5px 18px;}
			a:hover, a.on {
				color: #cc3333;
				background-color: #ffffff;}
		</style>
	</head>
	<body>
		<div id="page">
			<div id="logo">
				<img src="images/logo.gif" alt="The Analog Specialists">
			</div>
			<ul id="navigation">
				<li><a href="#" class="on">Home</a></li>
				<li><a href="#">For Sale</a></li>
				<li><a href="#">Repairs</a></li>
				<li><a href="#">About</a></li>
				<li><a href="#">Contact</a></li>
			</ul>
			<p><img src="images/puppy.jpg" alt="Fender Rhodes, Hohner Clavinet, and Wurlitzer EP200"></p>
			<p>We specialize in the sale and repair of classic keyboards, in particular the Fender Rhodes, Wurlitzer EP200, and Hohner Clavinet.
			</p>
		</div>
</body></html>
```

# List, Table and Form

## List
```css
/*List: bullet point styles*/
ul{list-style-type: none;}
ul{list-style-type: disc;}
ul{list-style-type: circle;}
ul{list-style-type: square;}

ol{list-style-type: decimal;}
ol{list-style-type: decimal-leading-zero;}
ol{list-style-type: lower-alpha;}
ol{list-style-type: upper-alpha;}
ol{list-style-type: lower-roman;}
ol{list-style-type: upper-roman;}

/*List: image for bullets*/
ul{list-style-image: url(images/logo.gif);}
li{margin: 10px 0px 0px 0px;}  /*vertical gap in lists*/

/*List: positioning the marker
marker sits inside or outside(default) of the box containing the points*/
ul{width:150px;}
li{margin: 10px;}
ul.illum{list-style-position:outside;}
ul.season{list-style-position:inside;}

/*List: shorthand*/
ul{list-style:inside circle; width:300px;}
li{margin: 10px 0px 0px 0px;}
```

## Table
```css
/*Table properties*/
table {
	width: 600px;}
th, td {
	padding: 7px 10px 10px 10px;}
th {
	text-transform: uppercase;
	letter-spacing: 0.1em;
	font-size: 90%;
	border-bottom: 2px solid #111111;
	border-top: 1px solid #999;
	text-align: left;}
tr.even {
	background-color: #efefef;}
tr:hover {
	background-color: #c3e6e5;}
.money {
	text-align: right;}

/*Table: border on empty cells*/
td{border: 1px solid #0088dd;
	padding:15px;}
table.one{empty-cells:show;}
table.two{empty-cells:hide;}
table.three{empty-cells:inherit;} /*table cells to obey the rules of the containing table*/

/*Table: gaps between cells*/
td{background-color: #0088dd;
	pdding:15px;
	border:2px solid #000000;}
table.one{border-spacing: 5px 15px;}
table.two{border-collapse: collapse;}
table.two{border-collapse: separate;} /*borders are detached from each other*/
```

## Forms
```css
/*Forms: Styling text inputs*/
input {
	font-size: 120%;
	color: #5a5854;
	background-color: #f2f2f2;
	border: 1px solid #bdbdbd;
	border-radius: 5px;
	padding: 5px 5px 5px 30px;
	background-repeat: no-repeat;
	background-position: 8px 9px;
	display: block;
	margin-bottom: 10px;}
input:focus, input:hover {
	background-color: #ffffff;
	border: 1px solid #b1e1e4;}
input#email {
	background-image: url("images/email.png");
	background-size:20px 20px;}
input#twitter {
	background-image: url("images/twitter.png");
	background-size:20px 20px;}
input#web {
	background-image: url("images/web.png");
	background-size:20px 20px;}

/*Forms: styling submit buttons*/
input {
	font-size: 120%;
	color: #5a5854;
	background-color: #f2f2f2;
	border: 1px solid #bdbdbd;
	border-radius: 5px;
	padding: 5px 10px 5px 10px;
	background-repeat: no-repeat;
	background-position: 8px 9px;
	display: block;
	margin-bottom: 10px;}
input#submit {
	color: #444444;
	text-shadow: 0px 1px 1px #ffffff;
	border-bottom: 2px solid #b2b2b2;
	background-color: #b9e4e3;
	background: -webkit-gradient(linear, left top, left bottom, from(#beeae9), to(#a8cfce));
	background: -moz-linear-gradient(top, #beeae9, #a8cfce);
	background: -o-linear-gradient(top, #beeae9, #a8cfce);
	background: -ms-linear-gradient(top, #beeae9, #a8cfce);}
input#submit:hover {
	color: #333333;
	border: 1px solid #a4a4a4;
	border-top: 2px solid #b2b2b2;
	background-color: #a0dbc4;
	background: -webkit-gradient(linear, left top, left bottom, from(#a8cfce), to(#beeae9));
	background: -moz-linear-gradient(top, #a8cfce, #beeae9);
	background: -o-linear-gradient(top, #a8cfce, #beeae9);
	background: -ms-linear-gradient(top, #a8cfce, #beeae9);}
```

```html
<!--Forms: Styling fieldsets & legends-->
<html><head>
		<title>Styling Fieldsets and Legends</title>
		<style type="text/css">
			* {
				font-family: Arial, Verdana, sans-serif;
				color: #665544;}
			input {
				border-bottom: 1px dotted #dcdcdc;
				border-top: none;
				border-right: none;
				border-left: none;
				padding: 5px;
				width: 280px;
				margin-bottom: 20px;}
			input:focus {
				border: 1px dotted #dcdcdc;
				outline: none;}
			input#submit {
				color: #ffffff;
				background-color: #665544;
				border: none;
				border-radius: 5px;
				width: 80px;}
			input#submit:hover {
				color: #665544;
				background-color: #efefef;}
			fieldset {
				width: 350px;
				border: 1px solid #dcdcdc;
				border-radius: 10px;
				padding: 20px;
				text-align: right;}
			legend {
				background-color: #efefef;
				border: 1px solid #dcdcdc;
				border-radius: 10px;
				padding: 10px 20px;
				text-align: left;
				text-transform: uppercase;}
		</style>
	</head>
	<body>
		<form>
			<fieldset>
				<legend>Newsletter</legend>
				<label for="name">Name: </label><input type="text" id="name">
				<label for="email">Email: </label><input type="text" id="email">
				<input type="submit" value="Subscribe" id="submit">
			</fieldset>
		</form>
</body></html>


<!--Forms: Aligning form controls PROBLEM & SOLUTION
	forms are not aligned to the left without css : set form width and align left-->
<html><head>
		<title>Aligning Form Controls - Solution</title>
		<style type="text/css">
			body {
				font-family: Arial, Verdana, sans-serif;}
			div {
				border-bottom: 1px solid #efefef;
				margin: 10px;
				padding-bottom: 10px;
				width: 260px;}
			.title {
				float: left;
				width: 100px;
				text-align: right;
				padding-right: 10px;}
			.submit {
				text-align: right;}
		</style>
	</head>
	<body>
		<form action="example.php" method="post">
			<div>
				<label for="name" class="title">Name:</label>
				<input type="text" id="name" name="name">
			</div>
			<div>
				<label for="email" class="title">Email:</label>
				<input type="email" id="email" name="email">
			</div>
			<div class="radio-buttons">
				<span class="title">Gender:</span>
				<input type="radio" name="gender" id="male" value="M">
				<label for="male">M</label>
				<input type="radio" name="gender" id="female" value="F">
				<label for="female">F</label><br>
			</div>
			<div class="submit">
				<input type="submit" value="Register" id="submit">
			</div>
		</form>
</body></html>
```

## Cursor styles
```html
<!--auto crosshair default pointer move text wait help url("cursor.gif")-->
<html><head>
		<style type="text/css">  a{cursor:move;}  </style>
	</head>
	<body>
		<a href="http://www.whitmanarchive.org">Walt Whitman</a>
</body></html>
```

## Web developer toolbar
<a href="www.chrispederick.com/work/web-developer">web developer tool</a>

## Example
```html
<html><head>
		<title>Lists, Tables and Forms</title>
		<style type="text/css">
			body {
				font-family: Arial, Verdana, sans-serif;
				font-size: 90%;
				color: #666666;
				background-color: #f8f8f8;}
			li {
				list-style-image: url("images/icon-plus.png");
				line-height: 1.6em;}
			table {
				border-spacing: 0px;}
			th, td {
				padding: 5px 30px 5px 10px;
				border-spacing: 0px;
				font-size: 90%;
				margin: 0px;}
			th, td {
				text-align: left;
				background-color: #e0e9f0;
				border-top: 1px solid #f1f8fe;
				border-bottom: 1px solid #cbd2d8;
				border-right: 1px solid #cbd2d8;}
			tr.head th {
				color: #fff;
				background-color: #90b4d6;
				border-bottom: 2px solid #547ca0;
				border-right: 1px solid #749abe;
				border-top: 1px solid #90b4d6;
				text-align: center;
				text-shadow: -1px -1px 1px #666666;
				letter-spacing: 0.15em;}
			td {
				text-shadow: 1px 1px 1px #ffffff;}
			tr.even td, tr.even th {
				background-color: #e8eff5;}
			tr.head th:first-child {
				-webkit-border-top-left-radius: 5px;
				-moz-border-radius-topleft: 5px;
				border-top-left-radius: 5px;}
			tr.head th:last-child {
				-webkit-border-top-right-radius: 5px;
				-moz-border-radius-topright: 5px;
				border-top-right-radius: 5px;}
			fieldset {
				width: 310px;
				margin-top: 20px;
				border: 1px solid #d6d6d6;
				background-color: #ffffff;
				line-height: 1.6em;}
			legend {
				font-style: italic;
				color: #666666;}
			input[type="text"] {
				width: 120px;
				border: 1px solid #d6d6d6;
				padding: 2px; q
				outline: none;}
			input[type="text"]:focus,
			input[type="text"]:hover {
				background-color: #d0e2f0;
				border: 1px solid #999999;}
			input[type="submit"] {
				border: 1px solid #006633;
				background-color: #009966;
				color: #ffffff;
				border-radius: 5px;
				padding: 5px;
				margin-top: 10px;}
			input[type="submit"]:hover {
				border: 1px solid #006633;
				background-color: #00cc33;
				color: #ffffff;
				cursor: pointer;}
			.title {
				float: left;
				width: 160px;
				clear: left;}
			.submit {
				width: 310px;
				text-align: right;}
		</style>
	</head>
	<body>
		<h1>Poetry Workshops</h1>
		<p>We will be conducting a number of poetry workshops and symposiums throughout the year.</p>
		<p>Please note that the following events are free to members:</p>
		<ul>
			<li>A Poetic Perspective</li>
			<li>Walt Whitman at War</li>
			<li>Found Poems and Outsider Poetry</li>
		</ul>
		<table>
			<tbody><tr class="head">
				<th></th>
				<th>New York</th>
				<th>Chicago</th>
				<th>San Francisco</th>
			</tr>
			<tr>
				<th>A Poetic Perspective</th>
				<td>Sat, 4 Feb 2012<br>11am - 2pm</td>
				<td>Sat, 3 Mar 2012<br>11am - 2pm</td>
				<td>Sat, 17 Mar 2012<br>11am - 2pm</td>
			</tr>
			<tr class="even">
				<th>Walt Whitman at War</th>
				<td>Sat, 7 Apr 2012<br>11am - 1pm</td>
				<td>Sat, 5 May 2012<br>11am - 1pm</td>
				<td>Sat, 19 May 2012<br>11am - 1pm</td>
			</tr>
			<tr>
				<th>Found Poems &amp; Outsider Poetry</th>
				<td>Sat, 9 Jun 2012<br>11am - 2pm</td>
				<td>Sat, 7 Jul 2012<br>11am - 2pm</td>
				<td>Sat, 21 Jul 2012<br>11am - 2pm</td>
			</tr>
			<tr class="even">
				<th>Natural Death: An Exploration</th>
				<td>Sat, 4 Aug 2012<br>11am - 4pm</td>
				<td>Sat, 8 Sep 2012<br>11am - 4pm</td>
				<td>Sat, 15 Sep 2012<br>11am - 4pm</td>
			</tr>
		</tbody></table>
		<form action="http://www.example.com/form.php" method="get">
			<fieldset>
				<legend>Register your interest</legend>
				<p><label class="title" for="name">Your name:</label>
					 <input type="text" name="name" id="name"><br>
					 <label class="title" for="email">Your email:</label>
					 <input type="text" name="email" id="email"></p>
				<p><label for="location" class="title">Your closest center:</label>
					 <select name="location" id="location">
						 <option value="ny">New York</option>
						 <option value="il">Chicago</option>
						 <option value="ca">San Francisco</option>
					 </select></p>
				<span class="title">Are you a member?</span>
				<label><input type="radio" name="member" value="yes"> Yes</label>
				<label><input type="radio" name="member" value="no"> No</label>
			</fieldset>
 	    <div class="submit"><input type="submit" value="Register"></div>
		</form>
</body></html>
```

# Layout

## Normal flow
```css
/*position: static;*/
body{
	width:750px;
	font-family: Arial,Verdana, sans-serif;
	color: #665544;}
h1{
	background-color: #efefef;
	padding:10px;}
p{width: 450px;}
```

there are :
* Relative positioning
* Absolute positioning
* Fixed positioning

## Relavtive positioning
moves an element in relation to where it would have been in normal flow

```css
p.example{
	position:relatvie; /*relative to normal flow*/
	top:10px;
	left:100px;}
```

## Absolute positioning
taken out of normal flow and no longer affects the positon of other elements on the page box offset specify where the elements should appear in relation to its containing element

```css
h1{
	position: absolute;
	top:0px;
	left: 500px;
	width:250px;}
```

## Fixed positioning
type of absolute positioning in relation to the browser window. It stays in the same exact place when a user scrolls down the page

```css
/*visible while scrolling*/
h1{
	position:fixed;
	top:0px;
	left: 500px;
	padding: 10px;
	margin:0px;
	width:100%;
	background-color: #efefef;}
```

## Overlapping elements
```css
/*higher z-index(stacking context), closer element is to the front*/
h1{
	position: fixed;
	top: 0px;
	left: 0px;
	margin: 0px;
	padding: 10px;
	width: 100%;
	background-color: #efefef;
	z-index: 10;}
p{
	position: relative;
	top: 70px;
	left: 70px;}
```

## Floating elements
The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible

```css
body {
	width: 750px;
	font-family: Arial, Verdana, sans-serif;
	color: #665544;}
blockquote {
	float: right; /*both float and width need to be specified*/
	width: 275px;

	font-size: 130%;
	font-style: italic;
	font-family: Georgia, Times, serif;
	margin: 0px 0px 10px 10px;
	padding: 10px;
	border-top: 1px solid #665544;
	border-bottom: 1px solid #665544;}
```

## Using Float to place elements side-by-side
Fourth paragraph is located below third due to short height of third paragraph.

```html
<html>
	<head>
		<title>Using Float to Place Elements Side-by-Side</title>
		<style type="text/css">
			body {
				width: 750px;
				font-family: Arial, Verdana, sans-serif;
				color: #665544;}
			p {
				width: 230px;
				float: left;
				margin: 5px;
				padding: 5px;
				background-color: #efefef;}
		</style>
	</head>
	<body>
		<h1>The Evolution of the Bicycle</h1>
		<div>
			<p>In 1817 Baron von Drais invented a walking machine that would help him get around the royal gardens faster.</p>
			<p>The device know as the Draisienne (or "hobby horse") was made of wood, and propelled by pushing your feet on the ground in a gliding movement.</p>
			<p>It was not seen as suitable for any place other than a well maintained pathway. </p>
			<p>In 1865, the velocipede (meaning "fast foot") attached pedals to the front wheel, but its wooden structure made it extremely uncomfortable. </p>
			<p>In 1870 the first all-metal machine appeared. The pedals were attached directly to the front wheel.</p>
			<p>Solid rubber tires and the long spokes of the large front wheel provided a much smoother ride than its predecessor.</p>
		</div>
	</body>
</html>
```

Setting the height of the paragraphs (as the height of the highest) is rarely suited to real world designs: use 'clear' property!

## Clearing Floats
```css
/*left or right side of the box should not touch any other elements
appearing in the same containing element*/
.clear{clear: left;}
.clear{clear: right;}

/*neither of both sides will touch*/
.clear{clear: both;}

/*elements can touch either side*/
.clear{clear: none;}
```

```html
<html>
	<head>
		<title>Clear</title>
		<style type="text/css">
			body {
				width: 750px;
				font-family: Arial, Verdana, sans-serif;
				color: #665544;}
			p {
				width: 230px;
				float: left;
				margin: 5px;
				padding: 5px;
				background-color: #efefef;}
			.clear {
				clear: left;}
		</style>
	</head>
	<body>
		<h1>The Evolution of the Bicycle</h1>
		<p>In 1817 Baron von Drais invented a walking machine that would help him get around the royal gardens faster.</p>
		<p>The device know as the Draisienne (or "hobby horse") was made of wood, and propelled by pushing your feet on the ground in a gliding movement.</p>
		<p>It was not seen as suitable for any place other than a well maintained pathway. </p>
		<p class="clear">In 1865, the velocipede (meaning "fast foot") attached pedals to the front wheel, but its wooden structure made it extremely uncomfortable.</p>
		<p>In 1870 the first all-metal machine appeared. The pedals were attached directly to the front wheel.
		</p><p>Solid rubber tires and the long spokes of the large front wheel provided a much smoother ride than its predecessor.</p>
	</body>
</html>
```

## Parents of Floated elements: PROBLEM
```css
/*If a containing element (div, containing p) only contains floated elements,
some browsers treat it as 0px tall resulting in collapsed border*/
div{border: 1px solid #665544;}
```

## Parents of Floated elements: SOLUTION
```css
/*1. overflow: auto; 2. width:100%;*/
div {border: 1px solid #665544;
	overflow: auto;
	width: 100%;}
```

## Creating multi-column layouts with Floats
div to represent each column

```html
<html><head>
		<title>Three Column Layout</title>
		<style type="text/css">
			body {
				width: 960px;
				font-family: Arial, Verdana, sans-serif;
				color: #665544;}
			.column1of3, .column2of3, .column3of3 {
				float: left; /*position column next to each other*/
				width: 300px; /*column width*/
				margin: 10px;} /*creates a gap between the columns*/
		</style>
	</head>
	<body>
		<h1>The Evolution of the Bicycle</h1>
		<div class="column1of3">
			<h3>The First Bicycle</h3>
			<p>In 1817 Baron von Drais invented a walking machine that would help him get around the royal gardens faster: two same-size in-line wheels, the front one steerable, mounted in a frame upon which you straddled. The device was propelled by pushing your feet against the ground, thus rolling yourself and the device forward in a sort of gliding walk.</p>
			<p>The machine became known as the Draisienne (or "hobby horse"). It was made entirely of wood. This enjoyed a short lived popularity as a fad, not being practical for transportation in any other place than a well maintained pathway such as in a park or garden.</p>
		</div>
		<div class="column2of3">
			<h3>Further Innovations</h3>
			<p>The next appearance of a two-wheeled riding machine was in 1865, when pedals were applied directly to the front wheel. This machine was known as the velocipede (meaning "fast foot") as well as the "bone shaker," since its wooden structure combined with the cobblestone roads of the day made for an extremely uncomfortable ride. They also became a fad and indoor riding academies, similar to roller rinks, could be found in large cities.</p>
			<p>In 1870 the first all-metal machine appeared. (Prior to this, metallurgy was not advanced enough to provide metal which was strong enough to make small, light parts out of.) The pedals were attached directly to the front wheel with no freewheeling mechanism. Solid rubber tires and the long spokes of the large front wheel provided a much smoother ride than its predecessor.</p>
		</div>
		<div class="column3of3">
			<h3>Bicycle Timeline</h3>
			<ul>
				<li>1817: Draisienne</li>
				<li>1865: Velocipede</li>
				<li>1870: High-wheel bicycle</li>
				<li>1876: High-wheel safety</li>
				<li>1885: Hard-tired safety</li>
				<li>1888: Pneumatic safety</li>
			</ul>
		</div>
</body></html>
```

## Screen size and resolution
higher resolution smaller texts

## Fixed width layouts
fixed size regardless of browser window size

```css
* {
	font-family: Arial, Verdana, sans-serif;
	color: #665544;
	text-align: center;}
body {
	width: 960px;
	margin: 0 auto;}
#content {
	overflow: auto;
	height: 100%;}
#nav, #feature, #footer {
	background-color: #efefef;
	padding: 10px;
	margin: 10px;}
.column1, .column2, .column3 {
	background-color: #efefef;
	width: 300px;
	float: left;
	margin: 10px;}
li {
	display: inline;
	padding: 5px;}
```

## Liquid layouts
stretch and contract as browser window size changes

```css
* {
	font-family: Arial, Verdana, sans-serif;
	color: #665544;
	text-align: center;}
body {
	width: 90%;
	margin: 0 auto;}
#content {
	overflow: auto;}
#nav, #feature, #footer {
	margin: 1%;}
.column1, .column2, .column3 {
	width: 31.3%;
	float: left;
	margin: 1%;}
.column3 {
	margin-right: 0%;}
li {
	display: inline;
	padding: 0.5em;}
#nav, #footer {
	background-color: #efefef;
	padding: 0.5em 0;}
#feature, .article {
	height: 10em;
	margin-bottom: 1em;
	background-color: #efefef;}
```

## Layout Grids
960 pixel grid

## CSS Framework
framework code provide code for common tasks in your project. e.g. 960 grid system (framwork)

## A Grid-based Layout using 960.gs framwork
* 960\_12\_col.css classes
* 		container_12 class: container for the whole page and indicate 12-column grid
*		clearfix class: inform browser height of the containing box since all floating elements
*		grid_12 class: to create a twelve-column wide block
*		grid_4 class: to create a four-column wide block

```html
<html><head>
		<title>Grid Layout</title>
		<link href="css/960_12_col.css" type="text/css" rel="stylesheet"/>
		<style>
			* {
				font-family: Arial, Verdana, sans-serif;
				color: #665544;
				text-align: center;}
			#nav, #feature, .article, #footer {
				background-color: #efefef;
				margin-top: 20px;
				padding: 10px 0px 5px 0px;}
			#feature, .article {
				height: 100px;}
			li {
				display: inline;
				padding: 5px;}
		</style>
	</head>
	<body>
		<div class="container_12 clearfix">
			<div id="header" class="grid_12">
				<h1>Logo</h1>
				<div id="nav">
					<ul>
						<li><a href="">Home</a></li>
						<li><a href="">Products</a></li>
						<li><a href="">Services</a></li>
						<li><a href="">About</a></li>
						<li><a href="">Contact</a></li>
					</ul>
				</div>
			</div>
			<div id="feature" class="grid_12">
				<p>Feature</p>
			</div>
			<div class="article grid_4">
				<p>Column One</p>
			</div>
			<div class="article grid_4">
				<p>Column Two</p>
			</div>
			<div class="article grid_4">
				<p>Column Three</p>
			</div>
			<div id="footer" class="grid_12">
				<p>&copy; Copyright 2011</p>
			</div>
		</div><!-- .container_12 -->
</body></html>
```

## Multiple style sheets
modular approach, split up CSS style rules into separate style sheets(fonts, layout, colors)

```html
<!--1. @import-->
<html><head>
		<title>Multiple Style Sheets - Import</title>
		<link rel="stylesheet" type="text/css" href="css/styles.css">
	</head>
	<body>
		<div id="page">
			<h1>Central Park Bike Hire</h1>
			<p class="intro">Rent a bicycle to ride around Central Park:</p>
			<table>
				<tbody><tr class="head">
					<th></th>
					<th>Per hour</th>
					<th>Per day</th></tr>
				<tr>
					<th>Cruiser</th>
					<td>$9</td>
					<td>$45</td>
				</tr>
				<tr>
					<th>21 Speed</th>
					<td>$15</td>
					<td>$50</td>
				</tr>
			</tbody></table>
			<h2>Where and When</h2>
			<h3>Loeb Boathouse</h3>
			<p>From April to November bicycles are available on first come first serve basis for riding in Central Park.</p>
			<h2>Deposits</h2>
			<h3>Cash or credit card</h3>
			<p>A $200 deposit is required for the hire of any of our bicycles.</p>
		</div>
</body></html>
```

```css
/* styles.css */
@import url("tables.css");
@import url("typography.css");
body {
	color: #666666;
	background-color: #f8f8f8;
	text-align: center;}
#page {
	width: 600px;
	text-align: left;
	margin-left: auto;
	margin-right: auto;
	border: 1px solid #d6d6d6;
	padding: 20px;}
h3 {
	color: #547ca0;}
```

```html
<!--2. link: the last link will take precedence over previous links-->
<head>
		<title>Multiple Style Sheets - Link</title>
		<link rel="stylesheet" type="text/css" href="css/site.css">
		<link rel="stylesheet" type="text/css" href="css/tables.css">
		<link rel="stylesheet" type="text/css" href="css/typography.css">
</head>
```

## Example
```html
<html><head>
		<title>Layout</title>
		<link rel="stylesheet" type="text/css" href="css/960_12_col.css">
		<style type="text/css">
			@font-face {
				font-family: 'QuicksandBook';
				src: url('fonts/Quicksand_Book-webfont.eot');
				src: url('fonts/Quicksand_Book-webfont.eot?#iefix') format('embedded-opentype'),
					url('fonts/Quicksand_Book-webfont.woff') format('woff'),
					url('fonts/Quicksand_Book-webfont.ttf') format('truetype'),
					url('fonts/Quicksand_Book-webfont.svg#QuicksandBook') format('svg');
				font-weight: normal;
				font-style: normal;}
			body {
				color: #ffffff;
				background: #413f3b url("images/bg.jpg");
				font-family: Georgia, "Times New Roman", Times, serif;
				font-size: 90%;
				margin: 0px;
				text-align: center;}
			a {
				color: #b5c1ad;
				text-decoration: none;}
			a:hover {
				color: #ffffff;}
			.header {
				background-image: url("images/bg-header.jpg");
				padding: 0px 0px 0px 0px;
				height: 100px;
				position: fixed;
				top: 0px;
				width: 100%;
				z-index: 50;}
			.nav {
				float: right;
				font-family: QuicksandBook, Helvetica, Arial, sans-serif;
				padding: 45px 0px 0px 0px;
				text-align: right;}
			.wrapper {
				width: 960px;
				margin: 0px auto;
				background-image: url("images/bg-triangle.png");
				background-repeat: no-repeat;
				background-position: 0px 0px;
				text-align: left;}
			.logo {
				margin-bottom: 20px;}
			h1, h2 {
				font-family: QuicksandBook, Helvetica, Arial, sans-serif;
				font-weight: normal;
				text-transform: uppercase;}
			h1 {
				font-size: 240%;
				margin-top: 140px;}
			.date {
				font-family: Arial, Helvetica, sans-serif;
				font-size: 75%;
				color: #b5c1ad;}
			.intro {
				clear: left;
				font-size: 90%;
				line-height: 1.4em;}
			.main-story {
				background-image: url("images/triangles.png");
				background-repeat: no-repeat;
				background-position: 122px 142px;
				height: 570px;}
			.more-articles {
				border-top: 1px solid #ffffff;
				padding: 10px;}
			.more-articles p {
				border-bottom: 1px solid #807c72;
				padding: 5px 0px 15px 0px;
				font-size: 80%;}
			.more-articles p:last-child {
				border-bottom: none;}
			.footer {
				clear: both;
				background: rgba(0, 0, 0, 0.2);
				padding: 5px 10px;}
			.footer p {
				font-family: Helvetica, Arial, sans-serif;
				font-size: 75%;
				text-align: right;}
			.footer a {
				color: #807c72;}
		</style>
	</head>
	<body>
		<div class="header">
			<div class="container_12">
				<div class="grid_5">
					<img src="images/logo.png" alt="Pedal Faster - The modern bicycle magazine" width="216" height="37" class="logo">
					<img src="images/header-triangle.png" alt="" width="116" height="100">
				</div>
				<div class="nav grid_7">
					<a href="">home</a> / <a href="">news</a> / <a href="">archives</a> / <a href="">about</a> / <a href="">contact</a>
				</div>
			</div>
		</div>
		<div class="wrapper">
			<div class="main-story container_12">
				<div class="grid_6 push_6">
					<h1><a href="">Fixed Gear Forever</a></h1>
				</div>
				<div class="intro grid_3 push_9">
					<p class="date">16 APRIL 2011</p>
					<p>The veloheld combines minimalist design with superb quality. Devoid of excessive graphics and gear shift components, the veloheld product range delights us with its beauty and simplicity. The black and white (yin and yang?) bicycles feature a short wheelbase, a single gear and a narrow handlebar... All you need to explore the city streets.</p>
					<p>For those who want to create their bike themselves, the veloheld frames come in three sizes and two colours and are the perfect starting point. <a href="">Continue reading...</a></p>
				</div>
			</div><!-- .main-story -->
			<div class="more-articles container_12">
				<h2 class="grid_12"><a href="">More Articles</a></h2>
				<div class="grid_3">
					<img src="images/more1.jpg" alt="The road ahead" width="220" height="125">
					<p><a href="">On the Road: From the fixed gear fanatic's point of view</a></p>
					<p><a href="">Brand History: Pashley Cycles - hand-built in England</a></p>
					<p><a href="">Frame Wars: Innovations in cycle manufacture and repair</a></p>
				</div>
				<div class="grid_3">
					<img src="images/more2.jpg" alt="Sketchbook" width="220" height="125">
					<p><a href="">Touring Diary: A sketchbook in your basket</a></p>
					<p><a href="">Top Ten Newcomers for 2012: A peek at what's to come</a></p>
					<p><a href="">InnerTube: The best cycling videos on the web</a></p>
				</div>
				<div class="grid_3">
					<img src="images/more3.jpg" alt="Repair shop sign" width="220" height="125">
					<p><a href="">Product Review: All baskets were not created equal</a></p>
					<p><a href="">Going Public: Out &amp; about with the founder of Public</a></p>
					<p><a href="">Cycle Lane Defence: Know your rights</a></p>
				</div>
				<div class="grid_3">
					<img src="images/more4.jpg" alt="Schwinn Spitfire" width="220" height="125">
					<p><a href="">Bicycle Hall of Fame: The 1958 Schwinn Spitfire</a></p>
					<p><a href="">Reader Survey: Share your thoughts with us!</a></p>
					<p><a href="">Chain Gang: The evolution of the humble bike chain</a></p>
				</div>
			</div><!-- .more-articles -->
		</div><!-- .wrapper -->
		<div class="footer clearfix">
			<div class="container_12">
				<p class="grid_12"><a href="">Legal Information</a> | <a href="">Privacy Policy</a> | <a href="">Copyright &copy; Pedal Faster 2011</a></p>
			</div>
		</div>
</body></html>
```

# Images

## Sizes of images
```css
img.large{
	width: 500px;
	height:500px;
}
```

## Align images using CSS
float property can be used to move an element to the left or right of its containing block, allowing text to flow around it. Rather than using the \<img\> element's align attribute, web page authors are increasingly using the float property to align images.

```html
<img class="align-left medium" src="images/mag.jpg" alt="Magnolia"/>
<img class="align-right medium" src="images/mag.jpg" alt="Magnolia"/>
```
```css
img.align-left{
	float:left;
	margin-right:10px;
}
img.align-right{
	float:right;
	margin-left:10px;
}
img.medium{
	width:250px;
	height:250px;
}
```

## Centering images using CSS
By default, images are inline elements. This means that they flow within the surrounding text. In order to center an image, it should be turned into a block-level element using the display property with a value of block.

```html
<p><img src="images/mag.jpg" alt="Magnolia" class="align-center medium"/>Magnolia.</p>
```
```css
img.align-center {
	display: block;
	margin: 0px auto;
}
img.medium {
	width: 250px;
	height: 250px;
}
```

## Background images
```css
body{
	background-image: url("images/pattern.gif");} /*for body*/
p{
	background-image: url("images/pattern.gif");} /*for element*/
```

## Repeating images
```css
body {
	background-image: url("images/header.gif");
	background-repeat: repeat-x; /*repeat-x  repeat-y  no-repeat*/
	color: #665544;
	padding: 20px;}
h1 {
	color: white;}
```

## Attach images
The background-attachment property specifies whether a background image should stay in one position or move as the user scrolls up and down the page. 
```css
body {
	background-image: url("images/tulip.gif");
	background-repeat: no-repeat;
	background-attachment: fixed; /*fixed or scroll*/
	color: #665544;
	padding: 20px;}
```

## Background position
```css
body{
	background-image:url("images/tulip.gif");
	background-repeat: no-repeat;
	background-position: center top;
	/*[9 by 9] left top, left center, left bottom, etc...*/
	/*background-position: 50% 0%; same as 'center top'*/
	/*background-position: 0px 0px;*/}
```

## Background Shorthand
1. background-color
2. background-image
3. background-repeat
4. background-attachment
5. background-position

```css
body{
	background: #ffffff url("images/tulip.gif") no-repeat top right;}
```

## image rollovers & sprites
a link or button that changes to a second style when a user moves their mouse over it(rollover) and a third style when clicked(activated). When a single image is used for several different parts of an interface, it is known as a sprite.

```html
<html><head>
		<title>Image Rollovers and Sprites</title>
		<style type="text/css">
			a.button {
				height: 36px;
				background-image: url("images/button-sprite.jpg");
				text-indent: -9999px;
				display: inline-block;}
			a#add-to-basket {
				width: 174px;
				background-position: 0px 0px;}
			a#framing-options {
				width: 210px;
				background-position: -175px 0px;}
			a#add-to-basket:hover {
				background-position: 0px -40px;}
			a#framing-options:hover {
				background-position: -175px -40px;}
			a#add-to-basket:active {
				background-position: 0px -80px;}
			a#framing-options:active {
				background-position: -175px -80px;}
		</style>
	</head>
	<body>
		<a class="button" id="add-to-basket">Add to basket</a>
		<a class="button" id="framing-options">Framing options</a>

</body></html>
```

## CSS3: gradients
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Gradient</title>
		<style type="text/css">
			#gradient {
				/* fallback color */
				background-color: #66cccc;
				/* fallback image */
				background-image: url("images/fallback-image.png");
				/* Firefox 3.6+ */
				background-image: -moz-linear-gradient(#336666, #66cccc);
				/* Safari 4+, Chrome 1+ */
				background-image: -webkit-gradient(linear, 0% 0%, 0% 100%, from(#66cccc), to(#336666));
				/* Safari 5.1+, Chrome 10+ */
				background-image: -webkit-linear-gradient(#336666, #66cccc);
				/* Opera 11.10+ */
				background-image: -o-linear-gradient(#336666, #66cccc);
   				height: 150px;
				width: 300px;}
		</style>
	</head>
	<body>
		<div id="gradient">
		</div>
	</body>
</html>
```

## Example
```html
<!DOCTYPE html>
<html>
	<head>
		<title>Images</title>
		<style type="text/css">
			body {
				color: #665544;
				background-color: #d4d0c6;
				background-image: url("images/backdrop.gif");
				font-family: Georgia, "Times New Roman", serif;
				text-align: center;}
			.wrapper {
				width: 720px;
				margin: 0px auto;}
			.header {
				margin: 40px 0px 20px 0px;}
			.entry {
				width: 220px;
				float: left;
				margin: 10px;
				height: 198px;
				background-image: url("images/shadow.png");
				background-repeat: no-repeat;
				background-position: bottom;}
			figure {
				display: block;
				width: 202px;
				height: 170px;
				background-color: #e7e3d8;
				margin: 0;
				padding: 9px;
				text-align: left;}
			figure img {
				width: 200px;
				height: 150px;
				border: 1px solid #d6d6d6;}
			figcaption {
				background-image: url("images/icon.png");
				padding-left: 20px;
				background-repeat: no-repeat;}
		</style>
	</head>
	<body>
		<div class="wrapper">
			<div class="header">
				<img src="images/title.gif" alt="Galerie Botanique" width="456" height="122" />
				<p>Here is a selection of antique botanical prints held in our collection.</p>
			</div>
			<div class="entry">
				<figure><img src="images/print-01.jpg" alt="Helianthus" />
					<figcaption>Helianthus</figcaption>
				</figure>
			</div>
			<div class="entry">
				<figure><img src="images/print-02.jpg" alt="Passiflora" />
					<figcaption>Passiflora</figcaption>
				</figure>
			</div>
			<div class="entry">
				<figure><img src="images/print-03.jpg" alt="Nyctocalos" />
					<figcaption>Nyctocalos</figcaption>
				</figure>
			</div>
			<div class="entry">
				<figure><img src="images/print-04.jpg" alt="Polianthes" />
					<figcaption>Polianthes</figcaption>
				</figure>
			</div>
			<div class="entry">
				<figure><img src="images/print-05.jpg" alt="Ficus" />
					<figcaption>Ficus</figcaption>
				</figure>
			</div>
			<div class="entry">
				<figure><img src="images/print-06.jpg" alt="Dendrobium" />
					<figcaption>Dendrobium</figcaption>
				</figure>
			</div>
		</div>
	</body>
</html>
```

# HTML5 Layout

## Traditional HTML layouts
use \<div\> for each main section in a page

## New HTML5 layout elements
* \<header\> \<footer\>
* \<nav\>
* \<article\>
* \<aside\>
* \<section\>
* \<hgroup\>
* \<figure\> \<figcaption\>
* \<div\>

## Header Footer (HTML5)
First, top and bottom of the page
Second, Each individual \<article\> and \<section\> element can also have its own \<header\> and \<footer\> elements to hold the header or footer information for that section within the page. For example, on a page with several blog posts, each individual post can be thought of as a separate section. The \<header\> element can therefore be used to contain the title and date of each individual post, and the \<footer\> might contain links to share the article on social networking sites.

## Navigation (HTML5)
The \<nav\> element is used to contain the major navigational blocks on the site such as the primary site navigation.

## Article (HTML5)
The \<article\> is a container for any section of a page that could stand alone indepenent piece of content such as article, blog entry, comment, forum post. If a page contains several articles (or even summaries), each individual article would live inside its own \<article\> element. The \<article\> elements can even be nested inside each other. For example, a blog post might live inside one \<article\> element and each comment on the article could live inside its own child \<article\> element.

## Aside (HTML5)
The \<aside\> element has two purposes, depending on whether it is inside an \<article\> element or not. Inside an article, it might contain info related to the article. e.g. pullquote, glossary. Outside an article, container for content related to the entire page. e.g. links, other posts, searchbox, tweets.

## Section (HTML5)
Groups related contents together and each section(e.g. latest news, top products, newsletter sign up) would have its own heading. It may contain several distinct \<article\> elements that have a common theme or purpose. Alternatively, if you have a page with a long article, split up into sections. The \<section\> element should not be used as a wrapper for the entire page. A containing element for the entire page, is still best left to the \<div\> element.

## Heading Group (HTML5)
The purpose of the \<hgroup\> element is to group together a set of one or more \<h1\> through \<h6\> elements so that they are treated as one single heading.

## Figure (HTML5)
\<figure\> can be used to contain any content that is referenced from the main flow of an article (not just images) e.g. image, video, graph, diagram, code samples, text support for main body of an article. The article should still make sense if the content of the \<figure\> element were moved to another part of the page or even a differnt page. For this reason, it should only be used when the content simply references the element (and not for something that is absolutely integral to the flow of a page)

## div (HTML5)
\<div\> element will remain an important way to group together related elements, because you should not be using these new elements that you have just met for purposes other than those explicitly stated.

```html
<div class="wrapper">
	<header></header>
	<section></section>
	<aside></aside>
	<footer></footer>
</div>
```

## Linking around block-level elements (HTML5)
```html
<a href="introduction.html">
	<article></article>
</a>
```

## Helping older browsers understand
Older browsers that do not know the new HTML5 elements will automatically treat them as inline elements. Therefore, to help older browsers, you should include the line of CSS on the left which states which new elements should be rendered as block-level elements.

```css
header, section, footer, aside, nav, article, figure{
	display: block;}
```

Also, IE9 was the first version of Internet Explorer to allow CSS  rules to be associated with these new HTML5 layout elements. In order to style these elements using earlier versions of IE, you need to use a simple JavaScript known as the HTML5 shiv or HTML5 shim.

```html
<!--[if lt IE 9]>
	<script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
<![endif]-->
```

## Example
```html
<!DOCTYPE html>
<html>
	<head>
		<title>HTML5 Layout</title>
		<style type="text/css">
			header, section, footer, aside, nav, article, figure, figcaption {
				display: block;}
			body {
				color: #666666;
				background-color: #f9f8f6;
				background-image: url("images/dark-wood.jpg");
				background-position: center;
				font-family: Georgia, Times, serif;
				line-height: 1.4em;
				margin: 0px;}
			.wrapper {
				width: 940px;
				margin: 20px auto 20px auto;
				border: 2px solid #000000;
				background-color: #ffffff;}
			header {
				height: 160px;
				background-image: url("images/header.jpg");}
			h1 {
				text-indent: -9999px;
				width: 940px;
				height: 130px;
				margin: 0px;}
			nav, footer {
				clear: both;
				color: #ffffff;
				background-color: #aeaca8;
				height: 30px;}
			nav ul {
				margin: 0px;
				padding: 5px 0px 5px 30px;}
			nav li {
				display: inline;
				margin-right: 40px;}
			nav li a {
				color: #ffffff;}
			nav li a:hover, nav li a.current {
				color: #000000;}
			section.courses {
				float: left;
				width: 659px;
				border-right: 1px solid #eeeeee;}
			article {
				clear: both;
				overflow: auto;
				width: 100%;}
			hgroup {
				margin-top: 40px;}
			figure {
				float: left;
				width: 290px;
				height: 220px;
				padding: 5px;
				margin: 20px;
				border: 1px solid #eeeeee;}
			figcaption {
				font-size: 90%;
				text-align: left;}
			aside {
				width: 230px;
				float: left;
				padding: 0px 0px 0px 20px;}
			aside section a {
				display: block;
				padding: 10px;
				border-bottom: 1px solid #eeeeee;}
			aside section a:hover {
				color: #985d6a;
				background-color: #efefef;}
			a {
				color: #de6581;
				text-decoration: none;}
			h1, h2, h3 {
				font-weight: normal;}
			h2 {
				margin: 10px 0px 5px 0px;
				padding: 0px;}
			h3 {
				margin: 0px 0px 10px 0px;
				color: #de6581;}
			aside h2 {
				padding: 30px 0px 10px 0px;
				color: #de6581;}
			footer {
				font-size: 80%;
				padding: 7px 0px 0px 20px;}
		</style>
		<!--[if lt IE 9]>
		<script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
		<![endif]-->
	</head>
	<body>
		<div class="wrapper">
			<header>
				<h1>Yoko's Kitchen</h1>
				<nav>
					<ul>
						<li><a href="" class="current">home</a></li>
						<li><a href="">classes</a></li>
						<li><a href="">catering</a></li>
						<li><a href="">about</a></li>
						<li><a href="">contact</a></li>
					</ul>
				</nav>
			</header>
			<section class="courses">
				<article>
					<figure>
						<img src="images/bok-choi.jpg" alt="Bok Choi">
						<figcaption>Bok Choi</figcaption>
					</figure>
					<hgroup>
						<h2>Japanese Vegetarian</h2>
						<h3>Five week course in London</h3>
					</hgroup>
					<p>A five week introduction to traditional Japanese vegetarian meals, teaching you a selection of rice and noodle dishes.</p>
				</article>    
				<article>
					<figure>
						<img src="images/teriyaki.jpg" alt="Teriyaki sauce">
						<figcaption>Teriyaki Sauce</figcaption>
					</figure>
					<hgroup>
						<h2>Sauces Masterclass</h2>
						<h3>One day workshop</h3>
					</hgroup>
					<p>An intensive one-day course looking at how to create the most delicious sauces for use in a range of Japanese cookery.</p>
				</article>    
			</section>
			<aside>
				<section class="popular-recipes">
					<h2>Popular Recipes</h2>
					<a href="">Yakitori (grilled chicken)</a>
					<a href="">Tsukune (minced chicken patties)</a>
					<a href="">Okonomiyaki (savory pancakes)</a>
					<a href="">Mizutaki (chicken stew)</a>
				</section>
				<section class="contact-details">
					<h2>Contact</h2>
					<p>Yoko's Kitchen<br>
						27 Redchurch Street<br>
						Shoreditch<br>
						London E2 7DP</p>
				</section>
			</aside>
			<footer>
				&copy; 2011 Yoko's Kitchen
			</footer>
		</div><!-- .wrapper -->
	</body>
</html>
```

# Process and Design

# Practical Information

## Domain names & Hosting
so that people can see your site, you need to upload it to a web server.

* disk space: html css images scripts
* bandwidth: the amount of data the hosting company will send to your site's visitors; num of people visiting every pages of your site times the amount of disk space
* backups: in case of a server breaking
* email accounts: hosting company will provide email servers. check the size and num of mailbox
* server-side language and databases: PHP & MySQL db,  ASP.Net & SQL Server db
* check the review of the hosting companies

## FTP & Third party tools
FTP allows you to transfer files across the internet from you pc to web server. e.g. ftp://mydomain.com

* FTP applications: FileZilla FireFTP CuteFTP SmartFTP Transmit
* Third party tools: blogs(wordpress tumblr posterous), e-commerce(shopify bigcartel magento) email newsletter(campaignmonitor mailchimp) sns sharing btn(addthis addtoany)
