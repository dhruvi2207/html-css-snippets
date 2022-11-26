# Anchor element

The Anchor tag defines a hyperlink, which is used to link from one page to another.

The most important attribute of the Anchor element is the href attribute, which indicates the link's destination.

Example 1
```
<nav class="dropdownmenu">
  <ul>
    <li><a href="http://www.jochaho.com/wordpress/">Home</a></li>
    <li><a href="http://www.jochaho.com/wordpress/about-pritesh-badge/">About Me</a></li>
    <li><a href="#">Articles on HTML5 & CSS3</a>
      <ul id="submenu">
        <li><a href="http://www.jochaho.com/wordpress/difference-between-svg-vs-canvas/">Difference between SVG vs. Canvas</a></li>
        <li><a href="http://www.jochaho.com/wordpress/new-features-in-html5/">New features in HTML5</a></li>
        <li><a href="http://www.jochaho.com/wordpress/creating-links-to-sections-within-a-webpage/">Creating links to sections within a webpage</a></li>
      </ul>
    </li>
    <li><a href="http://www.jochaho.com/wordpress/category/news/">News</a></li>
    <li><a href="http://www.jochaho.com/wordpress/about-pritesh-badge/">Contact Us</a></li>
  </ul>
</nav>
```
CSS
```
.dropdownmenu ul, .dropdownmenu li {
	margin: 0;
	padding: 0;
}
.dropdownmenu ul {
	background: gray;
	list-style: none;
	width: 100%;
}
.dropdownmenu li {
	float: left;
	position: relative;
	width:auto;
}
.dropdownmenu a {
	background: #30A6E6;
	color: #FFFFFF;
	display: block;
	font: bold 12px/20px sans-serif;
	padding: 10px 25px;
	text-align: center;
	text-decoration: none;
	-webkit-transition: all .25s ease;
	-moz-transition: all .25s ease;
	-ms-transition: all .25s ease;
	-o-transition: all .25s ease;
	transition: all .25s ease;
}
.dropdownmenu li:hover a {
	background: #000000;
}
#submenu {
	left: 0;
	opacity: 0;
	position: absolute;
	top: 35px;
	visibility: hidden;
	z-index: 1;
}
li:hover ul#submenu {
	opacity: 1;
	top: 40px;	/* adjust this as per top nav padding top & bottom comes */
	visibility: visible;
}
#submenu li {
	float: none;
	width: 100%;
}
#submenu a:hover {
	background: #DF4B05;
}
#submenu a {
	background-color:#000000;
}
```
---
Example2

Html
```
<canvas id="c"></canvas>

<div id="info">
  <div id="top">
    <a id="close" href="">&times;</a>
  </div>
  <p>
    <br>- Tear the cloth with your mouse
    <br>
    <br>- Right click and drag to cut
    <br>
    <br>
    <br>
    <div class="center">
      <a id="github" target="_blank" href="https://github.com/dissimulate/Tearable-Cloth">GitHub</a>&nbsp;<!--span class="bull">&bull;</span>&nbsp;<a id="twitter" target="_blank" href="https://twitter.com/abro_oks">@abro_oks</a-->
  </div>
    <br>
  </p>
</div>
```
 example2
 
 CSS

```
* {
    margin: 0;
    overflow: hidden;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    -o-user-select: none;
    user-select: none;
}
body {
    background: #F2F2F2;
}
#c {
    display: block;
    margin: 20px auto 0;
}
#info {
    position: absolute;
    left: -1px;
    top: -1px;
    width: auto;
    max-width: 420px;
    height: auto;
    background: #f8f8f8;
    border-bottom-right-radius: 10px;
    border:1px solid #ccc;
}
#top {
    background: #fff;
    width: 100%;
    height: auto;
    position: relative;
    border-bottom: 1px solid #eee;
}
p {
    font-family: Arial, sans-serif;
    color: #666;
    text-align: justify;
    font-size: 16px;
    margin: 0px 16px;
}
#github, #twitter {
  color:#3377ee;
  font-family: Helvetica, Arial, sans-serif;
  font-size: 14px;
  margin: 0 auto;
  text-align: center;
  text-decoration:none;
}
.center {
  text-align: center;
}
#net {
  text-align:center;
  white-space:nowrap;
  font-size:19px;
  background:rgba(0,0,0,0.1);
  padding:8px 12px;
  border-radius:8px;
  display:block;
  color:#888;
}
#net > span {
  color:#3377ee;
  font-family: Helvetica, Arial, sans-serif;
  font-size: 14px;
  display: block;
  margin: 0 auto;
  text-align: center;
  text-decoration:none;
}
a {
    font-family: sans-serif;
    color: #444;
    text-decoration: none;
    font-size: 20px;
}
#site {
    float: left;
    margin: 10px;
    color: #ff9900;
  border-bottom: 1px dashed #ccc;
  padding-bottom:3px
}
#site:hover {
    color: #ffaa11;
}
#close {
    float: right;
    margin: 10px;
}
#p {
    font-family: Verdana, sans-serif;
    position: absolute;
    right: 10px;
    bottom: 10px;
    color: #4099ff;
    border: 1px dashed #4099ff;
    padding: 4px 8px;
}

#new {
  width: 100%;
  text-align: center;
  font-size: 18px;
  font-family: Helvetica;
  margin-top: 12px;
}

#new a {
  font-size: 20px;
  color: #4099ff;
}

.bull {
  opacity: 0.3;
  margin: 0 6px;
  font-size: 14px;
}
```
---

