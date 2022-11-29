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
# Abbarviation element

The abbrevation tag defines an abbreviation or an acronym, like "HTML", "CSS", "Mr.", "Dr.", "ASAP", "ATM".

Tip: Use the global title attribute to show the description for the abbreviation/acronym when you mouse over the element.


HTML

example1
```

<ol class="periodic-table">
<li class="hydrogen">
    <abbr title="Hydrogen">H</abbr>
</li>
<li id="helium" class="noble-gas">
    <abbr title="Helium">He</abbr>
    <span>2</span>
</li>
<li class="alkali">
    <abbr title="Lithium">Li</abbr>
</li>
<li class="alkaline">
    <abbr title="Beryllium">Be</abbr>
</li>
<li id="boron" class="metalloid">
    <abbr title="Boron">B</abbr>
</li>
<li class="polyatomic-non-metal">
    <abbr title="Carbon">C</abbr>
</li>
<li class="diatomic-nonmetal">
    <abbr title="Nitrogen">N</abbr>
</li>
<li class="diatomic-nonmetal">
    <abbr title="Oxygen">O</abbr>
</li>
<li class="diatomic-nonmetal">
    <abbr title="Fluorine">F</abbr>
</li>
<li class="noble-gas">
    <abbr title="Neon">Ne</abbr>
</li>
<li class="alkali">
    <abbr title="Sodium">Na</abbr>
</li>
<li class="alkaline">
    <abbr title="Magnesium">Mg</abbr>
</li>
<li id="aluminium">
    <abbr title="Aluminium">Al</abbr>
</li>
<li class="metalloid">
    <abbr title="Silicon">Si</abbr>
</li>
<li class="polyatomic-non-metal">
    <abbr title="Phosphorus">P</abbr>
</li>
<li class="polyatomic-non-metal">
    <abbr title="Sulphur">S</abbr>
</li>
<li class="diatomic-nonmetal">
    <abbr title="Chlorine">Cl</abbr>
</li>
<li class="noble-gas">
    <abbr title="Argon">Ar</abbr>
</li>
<li class="alkali">
    <abbr title="Potassium">K</abbr>
</li>
<li class="alkaline">
    <abbr title="Calcium">Ca</abbr>
</li>
<li>
    <abbr title="Scandium">Sc</abbr>
</li>
<li>
    <abbr title="Titanium">Ti</abbr>
</li>
<li>
    <abbr title="Vanadium">Ti</abbr>
</li>
<li>
    <abbr title="Chromium">Cr</abbr>
</li>
<li>
    <abbr title="Manganese">Mn</abbr>
</li>
<li>
    <abbr title="Iron">Fe</abbr>
</li>
<li>
    <abbr title="Cobalt">Co</abbr>
</li>
<li>
    <abbr title="Nickel">Ni</abbr>
</li>
<li>
    <abbr title="Copper">Cu</abbr>
</li>
<li>
    <abbr title="Zinc">Zn</abbr>
</li>
<li>
    <abbr title="Gallium">Ga</abbr>
</li>
<li class="metalloid">
    <abbr title="Germanium">Ge</abbr>
</li>
<li class="metalloid">
    <abbr title="Arsenic">As</abbr>
</li>
<li class="polyatomic-non-metal">
    <abbr title="Selenium">Se</abbr>
</li>
<li class="diatomic-nonmetal">
    <abbr title="Bromide">Br</abbr>
</li>
<li class="noble-gas">
    <abbr title="Krypton">Kr</abbr>
</li>
<li class="alkali">
    <abbr title="Rubidium">Rb</abbr>
</li>
<li class="alkaline">
    <abbr title="Strontium">Sr</abbr>
</li>
<li>
    <abbr title="Yttrium">Y</abbr>
</li>
<li>
    <abbr title="Zirconium">Zr</abbr>
</li>
<li>
    <abbr title="Niobium">Nb</abbr>
</li>
<li>
    <abbr title="Molybdenum">Mo</abbr>
</li>
<li>
    <abbr title="Technetium">Tc</abbr>
</li>
<li>
    <abbr title="Ruthenium">Ru</abbr>
</li>
<li>
    <abbr title="Rhodium">Ro</abbr>
</li>
<li>
    <abbr title="Palladium">Pd</abbr>
</li>
<li>
    <abbr title="Silver">Ag</abbr>
</li>
<li>
    <abbr title="Cadmium">Cd</abbr>
</li>
<li>
    <abbr title="Indium">In</abbr>
</li>
<li>
    <abbr title="Tin">Sn</abbr>
</li>
<li class="metalloid">
    <abbr title="Antimony">Sb</abbr>
</li>
<li class="metalloid">
    <abbr title="Tellurium">Te</abbr>
</li>
<li class="diatomic-nonmetal">
    <abbr title="Iodine">I</abbr>
</li>
<li class="noble-gas">
    <abbr title="Xenon">Xe</abbr>
</li>
<li class="alkali">
    <abbr title="Caesium">Cs</abbr>
</li>
<li class="alkaline">
    <abbr title="Barium">Ba</abbr>
</li>
<li class="lanthanide">
    <abbr title="Lanthanum">La</abbr>
</li>
<li id="cerium" class="lanthanide">
     <abbr title="Cerium">Ce</abbr>
</li>
<li class="lanthanide">
    <abbr title="Praseodymium">Pr</abbr>
</li>
<li class="lanthanide">
    <abbr title="Neodymium">Nd</abbr>
</li>
<li class="lanthanide">
    <abbr title="Promethium">Pm</abbr>
</li>
<li class="lanthanide">
    <abbr title="Samarium">Sm</abbr>
</li>
<li class="lanthanide">
    <abbr title="Europium">Eu</abbr>
</li>
<li class="lanthanide">
    <abbr title="Gadolinium">Gd</abbr>
</li>
<li class="lanthanide">
    <abbr title="Terbium">Td</abbr>
</li>
<li class="lanthanide">
    <abbr title="Dysprosium">Dy</abbr>
</li>
<li class="lanthanide">
    <abbr title="Holmium">Ho</abbr>
</li>
<li class="lanthanide">
    <abbr title="Erbium">Er</abbr>
</li>
<li class="lanthanide">
    <abbr title="Thulium">Tm</abbr>
</li>
<li class="lanthanide">
    <abbr title="Ytterbium">Yb</abbr>
</li>
<li class="lanthanide">
    <abbr title="Lutetium">Lu</abbr>
</li>  
<li id="hafnium">
    <abbr title="Hafnium">Hf</abbr>
</li>
<li>
    <abbr title="Tantalum">Ta</abbr>
</li>
<li>
    <abbr title="Tungsten">W</abbr>
</li>
<li>
    <abbr title="Rhenium">Re</abbr>
</li>
<li>
    <abbr title="Osmium">Os</abbr>
</li> 
<li>
    <abbr title="Iridium">Ir</abbr>
</li>
<li>
    <abbr title="Platinum">Pt</abbr>
</li>
<li>
    <abbr title="Gold">Au</abbr>
</li>
<li>
    <abbr title="Mercury">Hg</abbr>
</li>
<li>
    <abbr title="Thallium">Tl</abbr>
</li>
<li>
    <abbr title="Lead">Pb</abbr>
</li>
<li>
    <abbr title="Bismuth">Bi</abbr>
</li>
<li>
    <abbr title="Polonium">Po</abbr>
</li>
<li class="metalloid">
    <abbr title="Astatine">At</abbr>
</li>
<li class="noble-gas">
    <abbr title="Radon">Rn</abbr>
</li>
<li class="alkali">
    <abbr title="Francium">Fr</abbr>
</li>
<li class="alkaline">
    <abbr title="Radium">Ra</abbr>
</li>
<li class="actinide">
    <abbr title="Actinium">Ac</abbr>
</li>
<li class="actinide" id="thorium" >
    <abbr title="Thorium">Th</abbr>
</li>
<li class="actinide">
    <abbr title="Protactinium">Pa</abbr>
</li>
<li class="actinide">
    <abbr title="Uranium">U</abbr>
</li>
<li class="actinide">
    <abbr title="Neptunium">Np</abbr>
</li>
<li class="actinide">
    <abbr title="Plutonium">Up</abbr>
</li>
<li class="actinide">
    <abbr title="Americium">Am</abbr>
</li>
<li class="actinide">
    <abbr title="Curium">Cm</abbr>
</li>
<li class="actinide">
    <abbr title="Berkelium">Bk</abbr>
</li>
<li class="actinide">
    <abbr title="Californium">Cf</abbr>
</li>
<li class="actinide">
    <abbr title="Einsteinium">Es</abbr>
</li>
<li class="actinide">
    <abbr title="Fermium">Fm</abbr>
</li>
<li class="actinide">
    <abbr title="Mendelevium">Md</abbr>
</li>
<li class="actinide">
    <abbr title="Nobelium">No</abbr>
</li>
<li class="actinide">
    <abbr title="Lawrencium">Lr</abbr>
</li>
<li id="rutherfordium">
    <abbr title="Rutherfordium">Rf</abbr>
</li>
<li>
    <abbr title="Dubnium">Db</abbr>
</li>
<li>
    <abbr title="Seaborgium">Sg</abbr>
</li>
<li>
    <abbr title="Bohrium">Bh</abbr>
</li>
<li>
    <abbr title="Hassium">Hs</abbr>
</li>
<li class="unknown">
    <abbr title="Meitnerium">Mt</abbr>
</li>
<li class="unknown">
    <abbr title="Darmstadtium">Ds</abbr>
</li>
<li class="unknown">
    <abbr title="Roentgenium">Rg</abbr>
</li>
<li>
    <abbr title="Copernicium">Cn</abbr>
</li>
<li class="unknown">
    <abbr title="Nihonium">Cn</abbr>
</li>
<li class="unknown">
    <abbr title="Flerovium">Fl</abbr>
</li>
<li class="unknown">
    <abbr title="Moscovium">Mc</abbr>
</li>
<li class="unknown">
    <abbr title="Livermorium">Lv</abbr>
</li>
<li class="unknown">
    <abbr title="Tennessine">Ts</abbr>
</li>
<li class="unknown">
    <abbr title="Oganesson">Og</abbr>
</li>
</ol>
```
CSS 

example1
```
@font-face {
  font-family: Phenomena;
  src:url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/4273/Phenomena-Regular.otf);
  font-weight: normal;
}

@font-face {
  font-family: Phenomena;
  src:url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/4273/Phenomena-Bold.otf);
  font-weight: bold;
}
* {
  box-sizing: border-box;
}
body {
  font-family: Phenomena, script;
  margin: 5vw;
  background: #111;
  color: #000;
  counter-reset: element;
}
.periodic-table {
  display: grid;
  grid-column-gap: .5vw;
  grid-row-gap: .5vw;
  padding-left: 0;
}
.periodic-table > li {
  display: flex;
  position: relative;
  justify-content: center;
  align-items: center;
  height: 4.5vw;
  border-radius: 3px;
  background: rgb(91, 194, 234);
  font-weight: bold;
}
.periodic-table > li:before {
  counter-increment: element; 
  content: counter(element);
  position: absolute;
  bottom: 5px;
  left: 6px;
  font-size: .9vw;
  font-weight: lighter;
}
.periodic-table > li abbr {
  font-size: 2.5vw;
}
#helium {
  grid-column-start: 18;
}
#boron, #aluminium {
  grid-column-start: 13;
}
#cerium, #thorium {
  grid-column-start: 4;
}
.periodic-table > li:nth-child(n+58):nth-last-child(n+48) {
  grid-row-start: 8;
}
.periodic-table > li:nth-child(n+90):nth-last-child(n+16) {
  grid-row-start: 9;
}
.periodic-table:before {
  display: block;
  content: '';
  grid-row: 8 / 10;
  grid-column: 1 / 4;
}
.periodic-table .noble-gas {
  background: rgb(234, 218, 36);
}
.periodic-table .diatomic-nonmetal {
  background: rgb(234, 179, 127);
}
.periodic-table .alkali {
  background: hsl(326, 52%, 84%);
}
.periodic-table .hydrogen {
  background: rgb(163, 199, 210);  
}
.periodic-table .alkaline {
  background: hsl(120, 52%, 84%);
}
.periodic-table .unknown {
  background: hsl(210, 2%, 73%);
}
.periodic-table .lanthanide {
  background: hsl(183, 54%, 84%);
}
.periodic-table .actinide {
  background: hsl(82, 60%, 56%);  
}
.periodic-table .metalloid {
  background: hsl(142, 60%, 56%);  
}
.periodic-table .polyatomic-non-metal {
  background: hsl(358, 60%, 56%);  
}

@media all and (max-width: 1100px) {
  #helium, #boron, #aluminium, #cerium, #thorium {
  grid-column-start: auto;
  }
  .periodic-table {
  grid-template-columns: 1fr 1fr 1fr;
  }
  .periodic-table > li abbr {
    font-size: 0;
  }
  .periodic-table > li {
    padding: 1rem;
  }
  .periodic-table > li abbr:after {
    content: attr(title);
    font-size: 2rem;
  }
  .periodic-table > li:before {
    font-size: 1rem;
  }
  .periodic-table > li:nth-child(n+58):nth-last-child(n+48) {
  grid-row-start: auto !important;
}
  .periodic-table > li:nth-child(n+90):nth-last-child(n+16) {
    grid-row-start: auto !important;
  }
  .periodic-table:before {
    display: none !important;
  }
}
@media all and (max-width: 750px) {
  body {
    margin: 2vw;
  }
  .periodic-table {
    grid-template-columns: 1fr 1fr;
  }
  .periodic-table > li {
    height: auto;
    font-size: 3vw;
  }
}
@media all and (max-width: 550px) {
  .periodic-table {
    grid-template-columns: 1fr;
  }
}

```

HTML

example2
```
!DOCTYPE html>
<html>
<body>

<h1>The abbr element</h1>

<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>

</body>
</html>

```
---

# Address element

The address tag defines the contact information for the author/owner of a document or an article.

The contact information can be an email address, URL, physical address, phone number, social media handle, etc.

The text in the address element usually renders in italic, and browsers will always add a line break before and after the address element.

HTML

example1

```
<address>
Written by <a href="mailto:webmaster@example.com">Ahmet Hakan</a>.<br> 
Visit us at:<br>
ahmethakanbesel.com.tr<br>
Box 564, Disneyland<br>
USA
</address>
```
CSS
```
address { 
    display: block;
    font-style: italic;
}

```

HTML 

example2
```
<html>
   
   <head>
      <title>Address Example</title>
   </head>
   
   <body>
      <address>388A, Road No 22, Jubilee Hills -  Hyderabad</address>
   </body>
   
</html>

```
---



# Area element
 
 the area tag defines an area inside an image map (an image map is an image with clickable areas).

area elements are always nested inside a map tag.

HTML

example1

```
<!DOCTYPE html>
<html>
<body>

<h1>The map and area elements</h1>

<p>Click on the computer, the phone, or the cup of coffee to go to a new page and read more about the topic:</p>

<img src="workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="coffee.htm">
</map>

</body>
</html>

```
# Artical element

the article tag specifies independent, self-contained content.

An article should make sense on its own and it should be possible to distribute it independently from the rest of the site.

Potential sources for the article element:

Forum post,
Blog post,
News story

HTML

example1
```
<nav id="menu">
  <button class="menu_button left_button">&lt;</button>
  <button class="menu_button right_button">&gt;</button>
  <div id="menu_div">
    <article>
      <img src="http://ocpsoft.org/wp-content/uploads/2013/01/javascript_logo_unofficial-300x300.png?1628ff" />
      <h2>JavaScript</h2>
      <p>JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed. Source: Wikipedia</p>
    </article>
    <article>
      <img src="http://element-80.com/wp-content/uploads/php_grunge.png" />
      <h2>PHP</h2>
      <p>PHP is a server-side scripting language designed for web development but also used as a general-purpose programming language. PHP is now installed on more than 244 million websites and 2.1 million web servers. Source: Wikipedia</p>
    </article>
    <article>
      <img src="http://traas.org/images/blog/python_logo.png" />
      <h2>Python</h2>
      <p>Python is a general-purpose, high-level programming language whose design philosophy emphasizes code readability. Python's syntax allows programmers to express concepts in fewer lines of code than would be possible in languages such as C. Source: Wikipedia</p>
    </article>
    <article>
      <img src="http://wpmu.org/wp-content/uploads/2013/01/codepen.png" />
      <h2>Slider</h2>
      <p>You can easy add an article to this slider. Just write another article in html and JavaScript will count all articles and it will works fine. You can edit CSS as you want to get beautiful and easy to use slider.</p>
    </article>
    <!--Here add your new <article> tag-->
  </div>
</nav>

```
CSS

example1
```
article {
  display: inline-block;
  padding: 25px 70px 25px 60px;
  width: 670px;
  vertical-align: top;
}

article img {
  max-height: 250px;
  max-width: 250px;
  margin-right: 20px;
  margin-bottom: 300px;
  float: left;
}
```

---

HTML

example2

```
<html>
<head>

</head>
<body>

<h1>The article element - Styled with CSS</h1>

<article class="all-browsers">
  <h1>Most Popular Browsers</h1>
  <article class="browser">
    <h2>Google Chrome</h2>
    <p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!</p>
  </article>
  <article class="browser">
    <h2>Mozilla Firefox</h2>
    <p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
  </article>
  <article class="browser">
    <h2>Microsoft Edge</h2>
    <p>Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.</p>
  </article>
</article>

</body>
</html>

```

CSS

example2
```

.all-browsers {
  margin: 0;
  padding: 5px;
  background-color: lightgray;
}

.all-browsers > h1, .browser {
  margin: 10px;
  padding: 5px;
}

.browser {
  background: white;
}

.browser > h2, p {
  margin: 4px;
  font-size: 90%;
}
```

---

# Aside element

The aside tag defines some content aside from the content it is placed in.

The aside content should be indirectly related to the surrounding content.

Tip: The aside content is often placed as a sidebar in a document.

HTML

example1
```
<article>
  <p>
    The is a simple paragraph.
  </p>
  <aside>
    <h4>The Paragraph</h4>
    <p>This is something related with the paragraphs.</p>
  </aside>
  <p>
    This is another paragraph.
  </p>
</article>

```

HTML

example2
```
<h2>Examples of Using the &lt;aside&gt; Tag</h2>

<div class="examples">
  <div class="unstyled">
    <h3>Default Appearance</h3>
    <article>
      <p>A long article about America. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante.</p>
      <aside>
        <p> California, a western U.S. state, stretches from the Mexican border along the Pacific for nearly 900 miles. Its terrain includes cliff-lined beaches, redwood forest, the Sierra Nevada Mountains, Central Valley farmland and the Mojave Desert. </p>
      </aside>
      <p>Some more information about America. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo. </p>
    </article>
    <div class="styled">
      <h3>Styled Using CSS</h3>
      <article>
      <p>A long article about America. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante.</p>
      <aside>
        <p> California, a western U.S. state, stretches from the Mexican border along the Pacific for nearly 900 miles. Its terrain includes cliff-lined beaches, redwood forest, the Sierra Nevada Mountains, Central Valley farmland and the Mojave Desert. </p>
      </aside>
      <p>Some more information about America. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo. </p>
    </article>
    </div>
  </div>

  <p class="more">Read more about the <a href="http://tutorialio.com/html/aside-tag.php" target="_blank" class="foot-link">usage and attributes of the HTML <code>&lt;aside&gt;</code> Element</a> on <a href="https://twitter.com/tutorialio" target="_blank" class="foot-link">Tutorialio</a>.</p>
```
CSS

example2
```
* {
  box-sizing: border-box;
}

html {
  font-family: 'Lato';
  text-align: justify;
  font-size: 1.25em;
  margin: 20px;
  margin-top: 50px;
}

h2 {
  text-align: center;
  margin-top: 0;
  margin-bottom: 50px;
}

h3 {
  margin-top: 50px;
  padding-bottom: 10px;
  border-bottom: 1px solid black;
}

.foot-link {
  text-decoration: none;
  color: cornflowerblue;
}

.more {
  color: black;
  text-align: right;
  margin-top: 80px;
}

.examples .styled article aside {
  border: 2px solid orange;
  padding: 10px;
  border-radius: 10px;
}

.examples .styled article aside p{
  margin: 10px 0;
}

```
---

# Audio tag

The audio tag is used to embed sound content in a document, such as music or other audio streams.

The audio tag contains one or more source tags with different audio sources. The browser will choose the first source it supports.

The text between the audio and audio tags will only be displayed in browsers that do not support the audio element.

HTML

example1
```
<link href='https://fonts.googleapis.com/css?family=Allerta' rel='stylesheet'>


    <h2>Wellcome to Rofa Music store</h2>
    <div class="container-audio">
        <audio controls  loop autoplay>
                   <source src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/9473/new_year_dubstep_minimix.ogg" type="audio/ogg">
                   Your browser dose not Support the audio Tag
               </audio>
    </div>
    <div class="container-audio">
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
        <div class="colum1">
            <div class="row"></div>
        </div>
    </div>

```

CSS

example1
```
* {
    font-family: 'Allerta', arial, Tahoma;
    box-sizing: border-box;
}
body {
    background: linear-gradient(to left, #7700aa, #8800ff);
    text-align:center;
    color:#fff;
}
h3{
    text-shadow:1px 1px 1px #fff;
}
/* Start  styling the page */
.container-audio {
    width: 66%;
    height: auto;
    padding: 20px;
    border-radius: 5px;
    background-color: #eee;
    color: #444;
    margin: 20px auto;
    overflow: hidden;
}
audio {
  width:100%;
}
audio:nth-child(2), audio:nth-child(4), audio:nth-child(6) {
    margin: 0;
}
.container-audio .colum1 {
    width: 23px;
    height: 5em;
    border-radius: 5px;
    margin: 0 10px 0 0;
    display: inline-block;
    position: relative;
}
.container-audio .colum1:last-child {
    margin: 0;
}
.container-audio .colum1 .row {
    width: 100%;
    height: 100%;
    border-radius: 5px;
    background: linear-gradient(to up, #7700aa, #8800ff);
    position: absolute;
    -webkit-animation: Rofa 10s infinite ease-in-out;
    animation: Rofa 10s infinite ease-in-out;
    bottom: 0;
}
.container-audio .colum1:nth-of-type(1) .row {
    -webkit-animation-delay: 3.99s;
    animation-delay: 3.99s;
}
.container-audio .colum1:nth-of-type(2) .row {
    -webkit-animation-delay: 3.80s;
    animation-delay: 3.80s;
}
.container-audio .colum1:nth-of-type(3) .row {
    -webkit-animation-delay: 3.70s;
    animation-delay: 3.70s;
}
.container-audio .colum1:nth-of-type(4) .row {
    -webkit-animation-delay: 3.60s;
    animation-delay: 3.60s;
}
.container-audio .colum1:nth-of-type(5) .row {
    -webkit-animation-delay: 3.50s;
    animation-delay: 3.50s;
}
.container-audio .colum1:nth-of-type(6) .row {
    -webkit-animation-delay: 3.40s;
    animation-delay: 3.40s;
}
.container-audio .colum1:nth-of-type(7) .row {
    -webkit-animation-delay: 3.30s;
    animation-delay: 3.30s;
}
.container-audio .colum1:nth-of-type(8) .row {
    -webkit-animation-delay: 3.20s;
    animation-delay: 3.20s;
}
.container-audio .colum1:nth-of-type(9) .row {
    -webkit-animation-delay: 3.10s;
    animation-delay: 3.10s;
}
.container-audio .colum1:nth-of-type(10) .row {
    -webkit-animation-delay: 2.1s;
    animation-delay: 2.1s;
}
.container-audio .colum1:nth-of-type(11) .row {
    -webkit-animation-delay: 2.1s;
    animation-delay: 2.1s;
}
.container-audio .colum1:nth-of-type(12) .row {
    -webkit-animation-delay: 2.10s;
    animation-delay: 2.10s;
}
.container-audio .colum1:nth-of-type(13) .row {
    -webkit-animation-delay: 2.20s;
    animation-delay: 2.20s;
}
.container-audio .colum1:nth-of-type(14) .row {
    -webkit-animation-delay: 1.30s;
    animation-delay: 1.30s;
}
.container-audio .colum1:nth-of-type(15) .row {
    -webkit-animation-delay: 1.40s;
    animation-delay: 1.40s;
}
.container-audio .colum1:nth-of-type(16) .row {
    -webkit-animation-delay: 1.50s;
    animation-delay: 1.50s;
}
.container-audio .colum1:nth-of-type(17) .row {
    -webkit-animation-delay: 1.60s;
    animation-delay: 1.60s;
}
.container-audio .colum1:nth-of-type(18) .row {
    -webkit-animation-delay: 1.70s;
    animation-delay: 1.70s;
}
.container-audio .colum1:nth-of-type(19) .row {
    -webkit-animation-delay: 1.80s;
    animation-delay: 1.80s;
}
.container-audio .colum1:nth-of-type(20) .row {
    -webkit-animation-delay: 2s;
    animation-delay: 2s;
}

@-webkit-keyframes Rofa {
    0% {
        height: 0%;
        -webkit-transform: translatey(0);
        transform: translatey(0);
        background-color: yellow;
    }

    5% {
        height: 100%;
        -webkit-transform: translatey(15px);
        transform: translatey(15px);
        background-color: fuchsia;
    }
    10% {
        height: 90%;
        transform: translatey(0);
        -webkit-transform: translatey(0);
        background-color: bisque;
    }

    15% {
        height: 80%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    20% {
        height: 70%;
        -webkit-transform: translatey(0);
        transform: translatey(0);
        background-color: cornflowerblue;
    }
    25% {
        height: 0%;
        -webkit-transform: translatey(0);
        transform: translatey(0);
        background-color: cornflowerblue;
    }
    30% {
        height: 70%;
        -webkit-transform: translatey(0);
        transform: translatey(0);
        background-color: cornflowerblue;
    }
    35% {
        height: 0%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    40% {
        height: 60%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    45% {
        height: 0%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    50% {
        height: 50%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    55% {
        height: 0%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    60% {
        height: 40%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    65% {
        height: 0%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    70% {
        height: 30%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    75% {
        height: 0%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    80% {
        height: 20%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    85% {
        height: 0%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    90% {
        height: 10%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    95% {
        height: 5%;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
    100% {
        height: 0;
        -webkit-transform: translatey(0);
        transform: translatey(0);

        background-color: cornflowerblue;
    }
}

```
HTML

example2
```
<h2>Web Audio Api Equalizer</h2>
<div class="eq">
  <div class="controls">
    <label>Low Gain</label>
    <input type="range" value="100" step="1" min="0" max="100" oninput="changeGain(this.value, 'lowGain');"></input>
  </div>
  <div class="controls">
    <label>Mid Gain</label>
    <input type="range" value="100" step="1" min="0" max="100" oninput="changeGain(this.value, 'midGain');"></input>
  </div>
  <div class="controls">
    <label>High Gain</label>
    <input type="range" value="100" step="1" min="0" max="100" oninput="changeGain(this.value, 'highGain');"></input>
  </div>
</div>
<h3>André Michelle <a href="www.audiotool.com/track/volution/">Volution</a></h3>
<audio id="player" controls crossorigin>
  <source src="http://api.audiotool.com/track/volution/play.mp3" type="audio/mpeg">
  <source src="http://api.audiotool.com/track/volution/play.ogg" type="audio/ogg">
  Your browser does not support the audio tag.
</audio>

```
CSS

example2
```
html, body {
  font-size: 12px;
  font-family: "Open Sans";
  background: #EEE;
}

a {
  text-decoration: none;
  color: #999;
}

audio {
  display: block;
}

.eq {
  margin: 32px;
}

div.controls label {
  display: inline-block;
  text-align: right;
  width: 80px;
}

div.controls label, div.controls input {
    vertical-align: middle;
    padding: 0;
    margin: 0;
}

```
---

# bold text

The b tag specifies bold text without any extra importance.

example
```
<html>
<body>

<h1>The b element</h1>

<p>This is normal text - <b>and this is bold text</b>.</p>

</body>
</html>

```
---

# Base tag

The base tag specifies the base URL and/or target for all relative URLs in a document.

The base tag must have either an href or a target attribute present, or both.

There can only be one single base element in a document, and it must be inside the head element.

Example
```
<!DOCTYPE html>
<html>
<head>
  <base href="https://www.w3schools.com/" target="_blank">
</head>
<body>

<h1>The base element</h1>

<p><img src="images/stickman.gif" width="24" height="39" alt="Stickman"> - Notice that we have only specified a relative address for the image. Since we have specified a base URL in the head section, the browser will look for the image at "https://www.w3schools.com/images/stickman.gif".</p>

<p><a href="tags/tag_base.asp">HTML base tag</a> - Notice that the link opens in a new window, even if it has no target="_blank" attribute. This is because the target attribute of the base element is set to "_blank".</p>

</body>
</html>

```
---
# bdi element

BDI stands for Bi-Directional Isolation.

The bdi tag isolates a part of text that might be formatted in a different direction from other text outside it.

This element is useful when embedding user-generated content with an unknown text direction.

example1
```
<ul>
  <li>Kullanıcı: <bdi>arayüz</bdi>10</li>
  <li>Kullanıcı: <bdi>إيان</bdi>20</li>
</ul>


```
example2

HTML

```
<h2>Examples of Using the &lt;bdi&gt; Tag</h2>

<div class="examples">
  <div class="unstyled">
    <h3>Without &lt;bdi&gt;</h3>
    <p>User WeberXx : 12 posts.</p>
    <p>User HoberYx : 5 posts.</p>
    <p>User إيان : 3 posts.</p>
  </div>
  <div class="styled">
    <h3>With &lt;bdi&gt;</h3>
    <p>User <bdi>WeberXx</bdi> : 12 posts.</p>
    <p>User <bdi>HoberYx</bdi> : 5 posts.</p>
    <p>User <bdi>إيان</bdi> : 3 posts.</p>
  </div>
</div>

```
CSS 

example2
```
* {
  box-sizing: border-box;
}

html {
  font-family: 'Lato';
  text-align: justify;
  font-size: 1.25em;
  margin: 20px;
  margin-top: 50px;
}

h2 {
  text-align: center;
  margin-top: 0;
  margin-bottom: 50px;
}

h3 {
  margin-top: 50px;
  padding-bottom: 10px;
  border-bottom: 1px solid black;
}


```
---

# bdo element

BDO stands for Bi-Directional Override.

The bdo tag is used to override the current text direction.
    
HTML
example1
```
<h2>Examples of Using the &lt;bdo&gt; Tag</h2>
  
<div class="examples">
  <div class="unstyled">
    <h3>Normal and "rtl" &lt;bdo&gt;</h3>
    <p>Don't ever take a fence down until you know why it was put up.</p>
	<p><bdo dir="rtl">Don't ever take a fence down until you know why it was put up.</bdo></p>
  </div>

```
CSS 

example1
```
* {
  box-sizing: border-box;
}

html {
  font-family: 'Lato';
  text-align: justify;
  font-size: 1.25em;
  margin: 20px;
  margin-top: 50px;
}

h2 {
  text-align: center;
  margin-top: 0;
  margin-bottom: 50px;
}

h3 {
  margin-top: 50px;
  padding-bottom: 10px;
  border-bottom: 1px solid black;
}

```
HTML

example2
```
<bdo dir="rtl">
Bu metin  sağdan sola doğru devam edecek
</bdo>

```
---
# blockquote element

The blockquote tag specifies a section that is quoted from another source.

Browsers usually indent blockquote elements (look at example below to see how to remove the indentation).

HTML 

example1
```
<h1>Blockquote styling part 1</h1>
<p>Here is a simple and clean blockquote styling</p>
<blockquote>
  <p>Your time is limited, so don't waste it living someone else's life. Don't be trapped by dogma - which is living with the results of other people's thinking. Don't let the noise of others' opinions drown out your own inner voice. And most important, have the courage to follow your heart and intuition.<p>
  <span>By Steve Jobs</span>
 </blockguote>

```
CSS 

example1

```

body {
  color : #22313F;
}

blockquote {
  background: #f9f9f9;
  border-left: 10px solid #03C9A9;
  margin: 1.5em 10px;
  padding:10px;
}
blockquote:before {
	font-family : georgia;
  color: #6C7A89;
  content: open-quote;
  font-size: 60px;
  /* how to fix the quote position*/
  line-height: 0.1em;
  vertical-align: -0.4em;
}

blockquote p {
  display: inline;
  letter-spacing : 1px;
}

blockquote span {
  display : block;
  margin-top : 10px;
  margin-left : 10px;
  font-size : 15px;
  font-style:italic;
}
blockquote span:before {
  content : "-";
  margin-right : 3px;
}

```
HTML 

example2
```
<html>
<body>

<h1>The blockquote element</h1>

<p>Here is a quote from WWF's website:</p>

<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 50 years, WWF has been protecting the future of nature. The world's leading conservation organization, WWF works in 100 countries and is supported by 1.2 million members in the United States and close to 5 million globally.
</blockquote>

</body>
</html>

```
---
# body element

The body tag defines the document's body.

The body element contains all the contents of an HTML document, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.

Note: There can only be one body element in an HTML document.

example
```
<html>
<head>
<style>
body {
  color: green;
}
</style>
</head>
<body>

<h1>Hello world!</h1>
<p>This is some text.</p>
<p><a href="https://www.w3schools.com">Visit W3Schools.com!</a></p>

</body>
</html>

```
---

# br tag

The br tag inserts a single line break.

The br tag is useful for writing addresses or poems.

The br tag is an empty tag which means that it has no end tag.

example
```
<html>
<body>

<h1>A Poem</h1>

<p>Be not afraid of greatness.<br>
Some are born great,<br>
some achieve greatness,<br>
and others have greatness thrust upon them.</p>

<p><em>-William Shakespeare</em></p>

</body>
</html>

```
---
# button element

The button tag defines a clickable button.

Inside a button element you can put text (and tags like i, b, strong, br, img, etc.). That is not possible with a button created with the input element!

Tip: Always specify the type attribute for a button element, to tell browsers what type of button it is.

Tip: You can easily style buttons with CSS! Look at the examples below or visit our CSS Buttons tutorial.

HTML

example1
```
<button class="buttonfx" type="submit">Slide Down</button>
<button class="buttonfx slideleft">Slide Left</button>
<button class="buttonfx slidebottomleft">Slide Corner</button>
<button class="buttonfx angleinleft">Angle In</button>
<br />

<button class="buttonfx bouncein" type="submit">Bounce Down</button>
<button class="buttonfx slideleft bouncein">Bounce Left</button>
<button class="buttonfx slidebottomleft bouncein">Bounce Corner</button>
<button class="buttonfx angleinleft bouncein">Bounce Angle</button>

<br />
<button class="buttonfx curtaindown">Curtain Down</button>
<button class="buttonfx curtainup">Curtain Up</button>
<button class="buttonfx angleindouble" type="submit">Double Angle</button>
<button class="buttonfx doubletake">Double Take</button>

<p><b>Tutorial:</b> <a href="http://blog.dynamicdrive.com/popular-css-button-hover-effects-explained/">Popular CSS Button Hover Effects Explained</a></b>

```
CSS 

example1
```
.buttonfx{
  color: black; /* button text color */
  outline: none;
  background: transparent;
  border: none;
  border-bottom: 4px solid #eee;
  letter-spacing: 0.0625em;
  padding: 8px 10px; 
  text-transform: uppercase;
  font: bold 16px 'Bitter', sans-serif; /* use google font */
  line-height: 2;
  position: relative;
	display: inline-block;
  margin-right: 20px;
  margin-bottom: 20px;
  cursor: pointer;
	text-decoration: none; /* remove underline if using A instead of BUTTON tag */
  overflow: hidden;
  transition: all .5s;
}

/* //// Default effect: Slide from Top  //// */

.buttonfx:before,
.buttonfx:after{
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  right: 0;
  bottom: 0;
  height: 100%;
  background: #259f6c; /* onhover background color */
  z-index: -1;
  transform: translate3D(0,-100%,0); /* move elements above button so they don't appear initially */
  transition: all .5s;
}

.buttonfx:before{
  background: #fafcd6; /* button default background color */
  z-index: -2;
  transform: translate3D(0,0,0);
}

.buttonfx:hover{
	color: white;
}

.buttonfx:hover:after{
  transform: translate3D(0,0,0);
  transition: all .5s;
}

/* //// Slide Left  //// */

.slideleft:after{
  top: 0;
  z-index: -1;
  transform: translate3D(-101%,0,0);
}

.slideleft:hover:after{
  transform: translate3D(0,0,0);
  transition: all .5s;
}

/* //// Slide Corner  //// */

.slidebottomleft:after{
  transform: translate3D(-100%,100%,0);
}

.slidebottomleft:hover:after{
	transform: translate3D(0,0,0);
  transition: all .5s;
}

/* //// Angle In  //// */


.angleinleft:after{
  width: 200%;
  transform-origin: 0 bottom;
  transform: translate3D(-50%,0,0) rotate(-50deg);
}

.angleinleft:hover:after{
  transform: rotate(0deg);
  transition: all .5s;
}

/* //// Curtain Down  //// */

.curtaindown{
  border: 1px solid #eee;
  border-bottom: 4px solid #eee;
}

.curtaindown:before,
.curtaindown:after{
  background: #259f6c;
  transform: translate3D(0,-100%,0);
}

.curtaindown:after{
  transform: translate3D(0,100%,0);
}

.curtaindown:hover:before,
.curtaindown:hover:after{
  transform: translate3D(0,-50%,0);
  transition: all .5s;
}

.curtaindown:hover:after{
  transform: translate3D(0,50%,0);
}

/* //// Curtain Up  //// */

.curtainup{
  transform-style: preserve-3d;
}

.curtainup:before,
.curtainup:after{
  transform-origin: center center;
  transform: scale(1,0);
}


.curtainup:hover:before,
.curtainup:hover:after{
  transform: scale(1);
  border-radius: 0;
}

/* //// Double Angle In  //// */

.angleindouble{
  border: 1px solid #eee;
  border-bottom: 4px solid #eee;
}

.angleindouble:before{
  top: 0;
  left: 0;
  width: 150%;
  background: #259f6c;
  transform-origin: 0 bottom;
  transform:  translateX(-100%) rotate(-30deg);
}

.angleindouble:after{
  top: 0;
  left: auto;
  right: 0;
  width: 150%;
  transform-origin: right bottom;
  transform: translateX(100%) rotate(30deg);
}

.angleindouble:hover:before{
  left: 0;
  transform: rotate(0deg);
  transition: all .5s;
}

.angleindouble:hover:after{
  right: 0;
  transform: rotate(0deg);
  transition: all .5s;
}


/* //// Double Take  //// */

.doubletake:before,
.doubletake:after{
  width: 200%;
  background: #259f6c;
  transform-origin: 0 bottom;
  transform: translate3D(-50%,0,0) rotate(-50deg);
}

.doubletake:before{
  opacity: .4;
}

.doubletake:hover:before,
.doubletake:hover:after{
  transform: rotate(0deg);
  transition: all .25s;
}

.doubletake:hover:after{
  transition-delay: .25s;
}


/* #### Bounce classes #### */

.bouncein:hover:before,
.bouncein:hover:after{
  transition-timing-function: cubic-bezier(0.52, 1.64, 0.37, 0.66) !important;
}

```

HTML example2

```
<div class="container" style="padding-top:80px;">
  <div class="col-md-3">
    Trigger with navbar, a link, a button,
    <br>or even just set an automatic timer!
    <br>
    <br>
    <button type="button" class="btn btn-primary btn-lg" data-toggle="modal" data-target="#lab-slide-bottom-popup"> Launch demo modal </button>
  </div>
</div>

```
CSS 

example2
```
<div class="container" style="padding-top:80px;">
  <div class="col-md-3">
    Trigger with navbar, a link, a button,
    <br>or even just set an automatic timer!
    <br>
    <br>
    <button type="button" class="btn btn-primary btn-lg" data-toggle="modal" data-target="#lab-slide-bottom-popup"> Launch demo modal </button>
  </div>
</div>

```
---
# canvas tag

The canvas tag is used to draw graphics, on the fly, via scripting (usually JavaScript).

The canvas tag is transparent, and is only a container for graphics, you must use a script to actually draw the graphics.

Any text inside the canvas element will be displayed in browsers with JavaScript disabled and in browsers that do not support canvas.

HTML

example1
```
<canvas id="c" width="500" height="500"></canvas><br/>
<!-- <canvas id="cv" width="500" height="500"></canvas> -->
<button type="button" id="btn"> Export&Import SVG</button>
<button type="button" id="btn_edit"> Export&Import JSON </button>  
  
  <p>Export to SVG</p> 
 <div id="svg-tag"></div>
  
 <p>Import from SVG</p> 
 <canvas id="canvas-svg" width="500" height="500"></canvas>  
 <p>Import from JSON</p> 
 <canvas id="canvas" width="500" height="500"></canvas> 


```
CSS 

example1
```
body{
  background-color: #cccccc;
}

.lw { font-size: 60px; }
canvas{
  border-style: dashed;  
}
button{
  margin:30px;
}
div{
  border-style: solid;
  border-color: #98bf21;
}

```
HTML

example2
```
<div>
  <button id="btn1">Tween Simple Bezier</button> <button id="btn2">Tween Simple Bezier Curviness 1.5</button> <button id="btn3">Tween Quadratic Bezier</button>
</div>

<canvas id="myCanvas" width="220" height="220" style="border:1px solid #d3d3d3; background:#fff;margin-top:24.5px;">
Your browser does not support the HTML5 canvas tag.</canvas>

<div>
<canvas id="myCanvas2" width="220" height="220" style="border:1px solid #d3d3d3; background:#fff;margin-top:24.5px;">
Your browser does not support the HTML5 canvas tag.</canvas>
</div>

<div class="div2" id="div2"></div>
<div class="div3" id="div3"></div>
<div class="div1" id="div1"></div>

```
CSS 

example2
```
.div1, .div2{
	width:20px;
	height:20px;
	position:absolute;
	top:48px;
	left:450px;
	background:#00f;
	border-radius:50%;
}
.div2, .div3{
  width:20px;
  height:20px;
  position:absolute;
  top:60px;
  left:108px;
  border-radius:50%;
  background:#F00;
}
.div3{
  top:310px;
}

```
---

# caption tag

The caption tag defines a table caption.

The caption tag must be inserted immediately after the table tag.

Tip: By default, a table caption will be center-aligned above a table. However, the CSS properties text-align and caption-side can be used to align and place the caption.

HTML

example1
```
<table border="1">
  <caption>This is a caption Table</caption>
  <tr>
    <th>Title 1</th>
    <th>Title 2</th>
  </tr>
  <tr>
    <td>Name 1</td>
    <td>Description 1</td>
  </tr>
	  <tr>
    <td>Name 2</td>
    <td>Description 2</td>
  </tr>
	  <tr>
    <td>Name 3</td>
    <td>Description 3</td>
  </tr>
</table>

```
example2

```
<table>
  <caption>Aylık Gider</caption>
  <tr>
    <th>ay</th>
    <th>gider</th>
  </tr>
  <tr>
    <td>Ocak</td>
    <td>100 TL</td>
  </tr>
</table>

```
---

# center tag

The center tag was used in HTML4 to center-align text.

---
# cite element

The cite tag defines the title of a creative work (e.g. a book, a poem, a song, a movie, a painting, a sculpture, etc.).

Note: A person's name is not the title of a work.

The text in the cite element usually renders in italic.

example
```
<html>
<body>

<h1>The cite element</h1>

<img src="img_the_scream.jpg" width="220" height="277" alt="The Scream">
<p><cite>The Scream</cite> by Edward Munch. Painted in 1893.</p>

</body>
</html>

```
---
# code tag

The code tag is used to define a piece of computer code. The content inside is displayed in the browser's default monospace font.

Tip: This tag is not deprecated. However, it is possible to achieve richer effect by using CSS (see example below).

example1
```
<html>
<head>
<style>
code { 
  font-family: monospace;
}
</style>
</head>
<body>

<p>A code element is displayed like this:</p>

<code>A piece of computer code</code>

<p>Change the default CSS settings to see the effect.</p>

</body>
</html>

```
example2

HTML
```
<body>

<h1>The code element + CSS</h1>

<p>The HTML <code>button</code> tag defines a clickable button.</p>
<p>The CSS <code>background-color</code> property defines the background color of an element.</p>

</body>

```
CSS
```
code {
  font-family: Consolas,"courier new";
  color: crimson;
  background-color: #f1f1f1;
  padding: 2px;
  font-size: 105%;

}
```
---
# column element

The col tag specifies column properties for each column within a colgroup element.

The col tag is useful for applying styles to entire columns, instead of repeating the styles for each cell, for each row.

Example1

HTML
```
<div class="col-controls">
  <button class="add_column">Add columns <span>(+)</span></button>
  <button class="remove_column">Remove columns <span>(-)</span></button>
</div>
<table class="test-table">
  <colgroup>
    <col class="data" />
    <col class="data" />
    <col class="data" />
    <col class="data" />
    <col class="data" />
    <col class="data" />
    <col class="data" />
    <col class="name" />
  </colgroup>

  <tbody>
    <tr>
      <td>1</td>
      <td>2</td>
      <td>3</td>
      <td>4</td>
      <td>5</td>
      <td>6</td>
      <td>7</td>
      <td>I'm the last one <span>(min-width: 200px)</span></td>
    </tr>
    <tr>
      <td>1</td>
      <td>2</td>
      <td>3</td>
      <td>4</td>
      <td>5</td>
      <td>6</td>
      <td>7</td>
      <td>I'm the last element of the second row</td>
    </tr>
    <tr>
      <td>1</td>
      <td>2</td>
      <td>3</td>
      <td>4</td>
      <td>5</td>
      <td>6</td>
      <td>7</td>
      <td>I'm the last element of the third row</td>
    </tr>
    <tr>
      <td>1</td>
      <td>2</td>
      <td>3</td>
      <td>4</td>
      <td>5</td>
      <td>6</td>
      <td>7</td>
      <td>I'm the last element of the fourth row</td>
    </tr>
    <tr>
      <td>1</td>
      <td>2</td>
      <td>3</td>
      <td>4</td>
      <td>5</td>
      <td>6</td>
      <td>7</td>
      <td>I'm the last element of the fifth row</td>
    </tr>
  </tbody>
</table>

```
CSS
```
body {
  padding-top: 3.5em;
}
.col-controls {
  position: fixed;
  left: 1em;
  top: .5em;
}
table { 
  width: auto;
  min-width: 100%;
  table-layout: fixed;
}
col.data { width: 120px; }

col.name {
  //background: #f00;
  
}
.test-table {
  td {
    min-width: 110px;
    //white-space: nowrap;
    border: 1px solid #ededec;
    padding: .5em;
    color: #777;
    
    &:nth-child(odd) {
      background: #f7f7f7;
    }
    &:last-child {
      min-width: 200px;
      background: #19c8b1;
      color: #fff;
      border-color: #18af9b;
      span {
        color: #fff;
        white-space: nowrap;
      }
    }
    
    span {
      color: #999;
      font-weight: 100;
      font-size: .8em;
    }
  }
}

button {
  border: 1px solid #d36b4e;
  background: #ee7e5e;
  color: #fff;
  font-weight: 100;
  padding: .5em 1em;;
  span {
    font-weight: 700;
  }
}

```
HTML
example2
```
<table border="1">
<colgroup>
	<col span="2" style="background: green">
	<col>
	<col>
	<col style="background: red">
	<col>
</colgroup>
<tr>
	<th>title 1</th>
	<th>title 2</th>
	<th>title 3</th>
	<th>title 4</th>
	<th>title 5</th>
</tr>
<tr>
	<td>content 1</td>
	<td>content 2</td>
	<td>content 3</td>
	<td>content 4</td>
	<td>content 5</td>
</tr>
</table>

```
---
# column group tag

The colgroup tag specifies a group of one or more columns in a table for formatting.

The colgroup tag is useful for applying styles to entire columns, instead of repeating the styles for each cell, for each row.

example1
```
<table border="1">
<colgroup>
	<col span="2" style="background: green">
	<col>
	<col>
	<col style="background: red">
	<col>
</colgroup>
<tr>
	<th>title 1</th>
	<th>title 2</th>
	<th>title 3</th>
	<th>title 4</th>
	<th>title 5</th>
</tr>
<tr>
	<td>content 1</td>
	<td>content 2</td>
	<td>content 3</td>
	<td>content 4</td>
	<td>content 5</td>
</tr>
</table>

```
---
# data element

The data tag is used to add a machine-readable translation of a given content.

This element provides both a machine-readable value for data processors, and a human-readable value for rendering in a browser.

Tip: If the content is time- or date-related, use the time element instead.

example
```
<html>
<body>

<h1>The data element</h1>

<p>The following example displays product names but also associates each name with a product number:</p>

<ul>
  <li><data value="21053">Cherry Tomato</data></li>
  <li><data value="21054">Beef Tomato</data></li>
  <li><data value="21055">Snack Tomato</data></li>
</ul>

</body>
</html>

```
---
# Datalist tag
The datalist tag specifies a list of pre-defined options for an input element.

The datalist tag is used to provide an "autocomplete" feature for input elements. Users will see a drop-down list of pre-defined options as they input data.

The datalist element's id attribute must be equal to the input element's list attribute (this binds them together).

HTML 

example1
```
<h2>Examples of Using the &lt;datalist&gt; Tag</h2>

<div class="examples">
  <div class="unstyled">
    <h3>Trying Typing 'The' in the Input.</h3>
    <label>Choose a movie from this list:
<input list="movies" name="myMovie" /></label>
    <datalist id="movies">
  <option value="The Shawshank Redemption">
  <option value="The Godfather">
  <option value="The Dark Knight">
  <option value="12 Angry Men">
  <option value="Schindler's List">
  <option value="Pulp Fiction">
</datalist>
  </div>
</div>

```
 example2
```
<label for="favourite-sites">Select your favorite website!</label>
<input type="url" name="favourite-sites" id="favourite-sites" list="site-list"/>
<datalist id="site-list">
  <option value="https://www.google.com.au">
  <option value="http://www.reddit.com">
  <option value="http://www.sitepoint.com">
</datalist>

```
---
# dd tag
The dd tag is used to describe a term/name in a description list.

The dd tag is used in conjunction with dl (defines a description list) and dt (defines terms/names).

Inside a dd tag you can put paragraphs, line breaks, images, links, lists, etc.

example1
```
<h1>Basic Definition List</h1>
	<dl>
		<dt>Title 1</dt>
			<dd>First Description for Title 1</dd>
			<dd>Second Description for Title 1</dd>
		<dt>Title 2</dt>
			<dd>First Description for Title 2</dd>
			<dd>Second Description for Title 2</dd>
	</dl>

```
example2
```
<dl>
<dt>Can't you people take the law into your own hands?</dt>
        
<dd><p>Don't kid yourself, Jimmy. If a cow ever got the chance, he'd eat you and everyone you care about! When I held that gun in my hand, I felt a surge of power…like God must feel when he's holding a gun.</p></dd>

<dt>What good is money if it can't inspire terror in your fellow man? </dt> 

<dd><p>Aaah! Natural light! Get it off me! Get it off me! I don't like being outdoors, Smithers. For one thing, there's too many fat children.</p></dd>
       
<dt>Inflammable means flammable? </dt>
  
<dd><p> Look out, Itchy! He's Irish! You don't like your job, you don't strike. You go in every day and do it really half-assed. That's the American way.</p></dd>
       
<dt>He didn't give you gay, did he? Did he?!</dt>
  
<dd><p>TY'ever sat down and read this thing?</p></dd>
       
<dt>There's a *New* Mexico?</dt>
       
<dd><p>A woman is a lot like a refrigerator. Six feet tall, 300 pounds…it makes ice. Our differences are only skin deep, but our sames go down to the bone.</p></dd>
      
</dl>

```
---
# delete tag
The del tag defines text that has been deleted from a document. Browsers will usually strike a line through deleted text.


```
<html>
<head>
<style>
del {background-color: tomato;}
ins {background-color: yellow;}
</style>
</head>
<body>

<h1>The del and ins elements + CSS</h1>

<p>My favorite color is <del>blue</del> <ins>red</ins>!</p>

</body>
</html>

```
---
# detail tag
The details tag specifies additional details that the user can open and close on demand.

The details tag is often used to create an interactive widget that the user can open and close. By default, the widget is closed. When open, it expands, and displays the content within.

Any sort of content can be put inside the details tag. 

example
```
<details>
	<summary>This is a detail tag</summary>
	<p>Random content: Fat new smallness few supposing suspicion two. Course sir people worthy horses add entire suffer. How one dull get busy dare far. At principle perfectly by sweetness do. As mr started arrival subject by believe. Strictly numerous outlived kindness whatever on we no on addition. </p>
</details>

```
---
# defination tag

The dfn tag stands for the "definition element", and it specifies a term that is going to be defined within the content.

The nearest parent of the dfn tag must also contain the definition/explanation for the term.

example
```
<html>
<body>

<h1>The dfn element</h1>

<p><dfn>HTML</dfn> is the standard markup language for creating web pages.</p>

</body>
</html>

```
example2
```
<p>A <dfn>kiwi</dfn> is a...</p>

```
---
# dialog tag

The dialog tag defines a dialog box or subwindow.

The dialog element makes it easy to create popup dialogs and modals on a web page.

example1
```
<header class="box rad p1">Test Template</header>

<div class="container">
	<button class="field btn" id="submit">Submit</button>
</div>

<dialog id="modal" class="box rad bor p0 modal">
	<div class="flex borb p1">
		<div id="modalHeading"></div>
		<button id="closeModal" class="field iconbtn">&#x26CC;</button>
	</div>
	<div id="modalContents" class="p1 borb"></div>
	<div class="flex p1">
		<button id="cancelModal" class="field btn"></button>
		<button id="continueModal" class="field btn"></button>
	</div>
</dialog>

```
```
.modal {
	width: 90%;
	max-width: 640px;
	color: inherit;
}
```
example2
```
<div>
  <h1>HTML5 Dialog Sample</h1>
  <p>This sample shows how to use the HTML5 <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dialog">dialog</a> tag. </p>
  <p>Check support  browser <a href="http://caniuse.com/#search=dialog">here</a>.</p>
</div>

<div>
  <button id="open" class="blue">Show Dialog</button>
</div>

<div id="dialogBG"></div>

<dialog id="dialog">
  <h3>Are you sure?</h3>
  <p>This is a custom confirm dialog using HTML5
  <div>
    <button id="ok" class="green">OK</button>
    <button id="cancel" class="red">Cancel</button>
  </div>
</dialog>

```

```
dialog { 
  color: #3d3d3d;
  background-color: #ffff91;
  width: 35%;
  text-align: center;
  border: 2px solid #f3f3f3;
  border-radius: 6px;
  z-index: 999999;
}

dialog div { 
  display: flex;
}

dialog::backdrop { 
  background: rgba(0,0,0,0.9);
}


```
---

# Div tag
The div tag defines a division or a section in an HTML document.

The div tag is used as a container for HTML elements - which is then styled with CSS or manipulated with JavaScript.

The div tag is easily styled by using the class or id attribute.

Any sort of content can be put inside the div tag! 





HTML

example1
```
<div class="bubble">
  Alright people, let's do <strong>this one last time.</strong>
</div>

<!-- bubble highlighting something  -->
<div class="bubble bubble--highlight">
  Play dumb
</div>

<!-- tag with the name of the main character -->
<div class="tag">
  <strong>Hello</strong>
  <br />
  my name is
</div>

```
CSS 
```
@import url("https://fonts.googleapis.com/css?family=Dekko|Lato:900|Rock+Salt");

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  min-height: 100vh;
  width: 100%;
  background: #eee;
  /* center the content in the page (mainly horizontally) */
  display: grid;
  place-items: center;
  /* include the same texture used for the .bubble containers, but with notably less opacity */
  background: url('data:image/svg+xml;utf8,<svg width="100" height="100" transform="rotate(0)" opacity="0.2" version="1.1" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg"><g  fill="%23250E17"><circle cx="25" cy="25" r="12.5"/><circle cx="75" cy="75" r="12.5"/><circle cx="75" cy="25" r="12.5"/><circle cx="25" cy="75" r="12.5"/></g></svg>'),
    #c52754;
  background-size: 10px, 100%;
}

/* .bubble containers: add the texture above a solid background */
.bubble {
  /* cap the width */
  max-width: 500px;
  /* give ample whitespace around and inside of the container */
  margin: 2rem 0;
  padding: 0.2rem 1.25rem;
  text-align: center;
  font-family: "Dekko", cursive;
  text-transform: uppercase;
  font-size: 2rem;
  letter-spacing: 0.2rem;
  background: url('data:image/svg+xml;utf8,<svg width="100" height="100" transform="rotate(25)" opacity="0.3" version="1.1" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg"><g  fill="%23250E17"><circle cx="25" cy="25" r="12.5"/><circle cx="75" cy="75" r="12.5"/><circle cx="75" cy="25" r="12.5"/><circle cx="25" cy="75" r="12.5"/></g></svg>'),
    #fff;
  background-size: 12px, 100%;
  /* solid border */
  border: 0.4rem solid #000;
  /* position relative for the :before pseudo element */
  position: relative;
}

/* for the highlight container change the solid backgorund to a yellow-ish hue */
.bubble--highlight {
  background: url('data:image/svg+xml;utf8,<svg width="100" height="100" transform="rotate(25)" opacity="0.8" version="1.1" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg"><g  fill="%23d68810"><circle cx="25" cy="25" r="12.5"/><circle cx="75" cy="75" r="12.5"/><circle cx="75" cy="25" r="12.5"/><circle cx="25" cy="75" r="12.5"/></g></svg>'),
    #ffcd28;
  background-size: 13px, 100%;
  font-weight: 700;
}
/* for the highlight container always add an exclamation point */
.bubble--highlight:after {
  content: "!";
}
/* for every .bubble container add a solid background behind the container itself, slightly offset */
.bubble:before {
  content: "";
  position: absolute;
  left: -1rem;
  top: 0.15rem;
  width: 100%;
  height: 100%;
  /* with the same texture, but different color, for both the texture and the background */
  background: url('data:image/svg+xml;utf8,<svg width="100" height="100" transform="rotate(35)" opacity="1" version="1.1" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg"><g fill="%23250E17"><circle cx="25" cy="25" r="12.5"/><circle cx="75" cy="75" r="12.5"/><circle cx="75" cy="25" r="12.5"/><circle cx="25" cy="75" r="12.5"/></g></svg>'),
    #000;
  background-size: 12px, 100%;
  border: 0.4rem solid #000;
  z-index: -5;
}

/* for the tag, add a lot of whitespace below the string, to include the name through the pseudo element */
.tag {
  margin-bottom: 2rem;
  padding: 1rem 7.5rem 11rem;
  border-radius: 30px;
  font-size: 2rem;
  color: #fff;
  background: #f8012d;
  text-align: center;
  font-family: "Lato", sans-serif;
  box-shadow: 0 1px 15px -7.5px #000000;
  /* position relative for the pseudo element(s) */
  position: relative;
}
.tag strong {
  text-transform: uppercase;
  font-size: 3.5rem;
}
/* with the :before pseudo element include a solid white background */
.tag:before {
  content: "";
  position: absolute;
  top: 9rem;
  left: 2%;
  width: 96%;
  height: 9rem;
  background: #fff;
  /* border-radius mathing the .tag container */
  border-radius: 0 0 30px 30px;
}
/* with the :after pseudo element add the name of the character */
.tag:after {
  content: "Peter Parker";
  position: absolute;
  top: 11.25rem;
  left: 0;
  width: 100%;
  text-align: center;
  font-family: "Rock Salt", cursive;
  font-size: 2rem;
  letter-spacing: 0.25rem;
  font-weight: 300;
  font-weight: bold;
  color: #000;
}

```

HTML
example2
```
<head>
  <style>
    div {
      padding: 16px;
      background-color: #00FF00;
    }
  </style>
</head>
<body>
  <div>
    <h1>Title with a background color</h1>
  </div>
</body>

```
---
# dl tag

The dl tag defines a description list.

The dl tag is used in conjunction with dt (defines terms/names) and dd (describes each term/name).

HTML

example1
```
<link href='https://fonts.googleapis.com/css?family=Exo+2:400,900,300,700,500,100' rel='stylesheet' type='text/css'>
<dl class="clone">
<dt>First Name</dt>
	<dd>James</dd>
<dt>Last Name</dt>
	<dd>Matman</dd>
<dt>Job Title</dt>
	<dd>Chief Sandwich Eater</dd>
<dt>Favorite Color</dt>
	<dd>Lettuce Green</dd>
<dt>Wars or Trek?</dt>
	<dd>Trek</dd>
<dt>Team Name</dt>
	<dd>Digby Green</dd>
<dt>Date of Birth</dt>
	<dd>January 13, 1979</dd>
<dt>Dream Vacation City</dt>
	<dd>Gotham City</dd>
<dt>GPA</dt>
	<dd>3.1</dd>
<dt>Arbitrary Data</dt>
	<dd>RBX-12</dd>
</dl>
	
<!-- 
	definition lists as table rows. it's turtles all the way down. 
!-->
<dl>
<dt>First Name</dt>
	<dd>James</dd>
<dt>Last Name</dt>
	<dd>Matman</dd>
<dt>Job Title</dt>
	<dd>Chief Sandwich Eater</dd>
<dt>Favorite Color</dt>
	<dd>Lettuce Green</dd>
<dt>Wars or Trek?</dt>
	<dd>Trek</dd>
<dt>Porn Name</dt>
	<dd>Digby Green</dd>
<dt>Date of Birth</dt>
	<dd>January 13, 1979</dd>
<dt>Dream Vacation City</dt>
	<dd>Gotham City</dd>
<dt>GPA</dt>
	<dd>3.1</dd>
<dt>Arbitrary Data</dt>
	<dd>RBX-12</dd>
</dl>

<dl>
<dt>First Name</dt>
	<dd>The</dd>
<dt>Last Name</dt>
	<dd>Tick</dd>
<dt>Job Title</dt>
	<dd>Crimefighter Sorta</dd>
<dt>Favorite Color</dt>
	<dd>Blue</dd>
<dt>Wars or Trek?</dt>
	<dd>Wars</dd>
<dt>Porn Name</dt>
	<dd>John Smith</dd>
<dt>Date of Birth</dt>
	<dd>July 19, 1968</dd>
<dt>Dream Vacation City</dt>
	<dd>Athens</dd>
<dt>GPA</dt>
	<dd>N/A</dd>
<dt>Arbitrary Data</dt>
	<dd>Edlund, Ben (July 1996).</dd>
</dl>

<dl>
<dt>First Name</dt>
	<dd>Jokey</dd>
<dt>Last Name</dt>
	<dd>Smurf</dd>
<dt>Job Title</dt>
	<dd>Giving Exploding Presents </dd>
<dt>Favorite Color</dt>
	<dd>Smurflow</dd>
<dt>Wars or Trek?</dt>
	<dd>Smurf</dd>
<dt>Porn Name</dt>
	<dd>Smurflane Smurfmutt</dd>
<dt>Date of Birth</dt>
	<dd>Smurfuary Smurfteenth, 1945 </dd>
<dt>Dream Vacation City</dt>
	<dd>New Smurf City </dd>
<dt>GPA</dt>
	<dd>4.Smurf </dd>
<dt>Arbitrary Data</dt>
	<dd>One</dd>
</dl>

<dl>
<dt>First Name</dt>
	<dd>Cindy</dd>
<dt>Last Name</dt>
	<dd>Beyler </dd>
<dt>Job Title</dt>
	<dd>Sales Representative </dd>
<dt>Favorite Color</dt>
	<dd>Red </dd>
<dt>Wars or Trek?</dt>
	<dd>Wars </dd>
<dt>Porn Name</dt>
	<dd>Lori Quivey</dd>
<dt>Date of Birth</dt>
	<dd>July 5, 1956 </dd>
<dt>Dream Vacation City</dt>
	<dd>Paris </dd>
<dt>GPA</dt>
	<dd>3.4 </dd>
<dt>Arbitrary Data</dt>
	<dd>3451</dd>
</dl>

<dl>
<dt>First Name</dt>
	<dd>Captain </dd>
<dt>Last Name</dt>
	<dd>Cool </dd>
<dt>Job Title</dt>
	<dd>Tree Crusher </dd>
<dt>Favorite Color</dt>
	<dd>Blue</dd>
<dt>Wars or Trek?</dt>
	<dd>Wars </dd>
<dt>Porn Name</dt>
	<dd>Steve 42nd</dd>
<dt>Date of Birth</dt>
	<dd>December 13, 1982 </dd>
<dt>Dream Vacation City</dt>
	<dd>Las Vegas </dd>
<dt>GPA</dt>
	<dd>1.9 </dd>
<dt>Arbitrary Data</dt>
	<dd>Under the couch</dd>
</dl>
</div>

```
CSS example1
```
dt, dd {
	margin:0;
	padding:0;
	width:49%;
	float:left;
}
dt{
  font-weight:bold;
}

dl:nth-of-type(odd) dt, dl:nth-of-type(odd) dd { 
	background: #ffe8f1; 
}

.clone {
	display:none;
}

@media (min-width: 800px) {

	dt, dd {
		padding:.25em;
		border-right:1px solid #c00;
		border-bottom:1px solid #c00;
		width:auto;
		float:none;
	}
	
	.faux-table {
		display:table;
		position:relative;
		border-top:1px solid #c00;
		border-left:1px solid #c00;
	}
	
	dt, dl.clone dd {
		display:none;
	}
	dl, dl.clone {
		display:table-row;
	}
	dl.clone dt, dd {
		display:table-cell;
	}
	
	dl.clone dt {
		color:#ddd;
		background:#c00;
		text-align:center;
		font-weight:bold;
	}
}

```

HTML example2
```
<html>
<body>

<h1>The dl, dd, and dt elements</h1>

<p>These three elements are used to create a description list:</p>

<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>

</body>
</html>

```
---

# dt tag
The dt tag defines a term/name in a description list.

The dt tag is used in conjunction with dl (defines a description list) and dd (describes each term/name).

EXAMPLE
```
<html>
<body>

<h1>The dl, dd, and dt elements</h1>

<p>These three elements are used to create a description list:</p>

<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>

</body>
</html>

```
---

# em tag
The em tag is used to define emphasized text. The content inside is typically displayed in italic.

A screen reader will pronounce the words in em with an emphasis, using verbal stress.

example1 
```
<html>
<body>

<h1>The em element</h1>

<p>You <em>have</em> to hurry up!</p>

<p>We <em>cannot</em> live like this.</p>

</body>
</html>

```
example2
```
<html>
<head>
<style>
em { 
  font-style: italic;
}
</style>
</head>
<body>

<p>An em element is displayed like this:</p>

<em>Some emphasized text</em>

<p>Change the default CSS settings to see the effect.</p>

</body>
</html>

```
---

# embed tag
The embed tag defines a container for an external resource, such as a web page, a picture, a media player, or a plug-in application.

example1
```
<html>
<body>

<h1>The embed element</h1>

<embed type="text/html" src="snippet.html"  width="500" height="200">

</body>
</html>

```
example2
```
<html>
<body>

<embed type="video/webm" src="movie.mp4" width="400" height="300">
 
</body>
</html>

```
---
# fieldset tag
The fieldset tag is used to group related elements in a form.

The fieldset tag draws a box around the related elements.

example1
```
<html>
<body>

<h1>The fieldset element</h1>

<form action="/action_page.php">
 <fieldset>
  <legend>Personalia:</legend>
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email"><br><br>
  <label for="birthday">Birthday:</label>
  <input type="date" id="birthday" name="birthday"><br><br>
  <input type="submit" value="Submit">
 </fieldset>
</form>

</body>
</html>

```
example2 HTML
```
<h1> Soccer Registration </h1>

<form>
  <label>Name: </label>
    <input type="text" name="name">
  <label>Email: </label>
    <input type="email" name="_replyto">


  <fieldset>
      <legend>Experience</legend>
      <input type="radio" name="radExperience" id="radBeginner"/>
      <label for="radBeginner">Beginner</label>
      <input type="radio" name="radExperience"
id="radIntermediate"/>
      <label for="radIntermediate">Intermediate</label>
      <input type="radio" name="radExperience" id="radExperienced"/>
     <label for="radExperienced">Experienced</label>
  </fieldset>
  <input id="send-button" type="submit" value="Send">
</form>

```
example2 CSS 
```
form {
  max-width: 200px;
  padding: 20px;
  font-family: Arial;
}

input {
  display: block;
  padding: 4px;
}

#send-button {
  color: #fff;
  margin: 20px;
  background-color: #456789;
  border-radius: 10%;
  font-size: 16px;
  border: none;
  padding: 10px;
  
}

fieldset {
  margin: 15px;
  background-color: #ccc;
  border: none;
}

```
---
# figcaption element
The figcaption tag defines a caption for a figure element.

The figcaption element can be placed as the first or last child of the figure element.

HTML example1
```
<figure>
  <img src="https://picsum.photos/300/300?random" alt="Rendom picture">
  <figcaption>Looking for something? Rendom picture here.</figcaption>
</figure>

```
CSS example1
```
@import url('https://fonts.googleapis.com/css?family==Encode+Sans+Condensed');
body { 
  background: #ffffff; 
  font: 14px/1.6 'Encode Sans Condensed', sans-serif;
}


figure {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  img {
    display: block;
    border: 0px solid #00b3b3;
    width: 300px;
    height: 300px;
    box-shadow: 0 0 0 4px rgba(0, 0, 0, 0), 0 0 10px 4px rgba(0, 0, 0, 0.18);
  }
  figcaption {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 5;
    color: #e8e8e8;
    padding: 20px;
    transform: translate(-75%, -50%);
    background-color: #2b2b2b;
    border: 4px solid #505050;
    font-weight: 500;
    max-width: 300px;
    a{
      color: #e8e8e8;
      text-decoration: none;
      border-bottom: 2px solid #a0a0a0;
    }
    &::before {
      position: absolute;
      content: '';
      top: calc(100% - 25px);
      left: calc(100% + 3px);
      transform: rotate(45deg);
      transform-origin: left top;
      border-top: 20px solid transparent;
      border-bottom: 20px solid transparent;
      border-left: 50px solid #505050;
    }
    &::after {
      position: absolute;
      content: '';
      top: calc(100% - 22px);
      left: calc(100% - 1px);
      transform: rotate(45deg);
      transform-origin: left top;
      border-top: 15px solid transparent;
      border-bottom: 15px solid transparent;
      border-left: 40px solid #2b2b2b;
    }
  }
}
```

Example2 HTML
```
<figure>
<img src="http://cssinhtml.com/wp-content/uploads/2016/05/user_image.jpg" alt="This is a figure image">
<figcaption>This is the caption of the Image</figcaption>
</figure>
<br>
<br><a href="http://www.cssinhtml.com" target="_blank">Go to CSS in HTML</a>

```
---

# figure tag

The figure tag specifies self-contained content, like illustrations, diagrams, photos, code listings, etc.

While the content of the figure element is related to the main flow, its position is independent of the main flow, and if removed it should not affect the flow of the document.

Tip: The figcaption element is used to add a caption for the figure element.

example
```
<html>
<body>

<h1>The figure and figcaption element</h1>

<figure>
  <img src="pic_trulli.jpg" alt="Trulli" style="width:100%">
  <figcaption>Fig.1 - Trulli, Puglia, Italy.</figcaption>
</figure>

</body>
</html>

```
---
# footer element

The footer tag defines a footer for a document or section.

A footer element typically contains:

authorship information
copyright information
contact information
sitemap
back to top links
related documents
You can have several footer elements in one document.

HTML example1
```
<div class="wrap">
  <header>
    <a href="#">Boo</a>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Work</a></li>
        <li><a href="#">Contact</a></li>
        <li><a href="#">Us</a></li>
      </ul>
    </nav>
  </header>
  
  <main>
    <section class="hero">
      <h1>Boogey Monster</h1>
      <hr/>
      <p>A gorgeous layout that caught my eye on Dribbble.<br/>So I had to give it a go.<br/>Inspired by <a href="https://dribbble.com/shots/2897240-DESIGN-HOUSE">Baoan</a>.</p>
    </section>
    
    <section class="content">
      <h2>Bears</h2>
      <p>Viral whatever umami, mlkshk microdosing kombucha sartorial chicharrones 8-bit meditation twee next level. Tofu wayfarers retro forage kale chips humblebrag, occupy banh mi +1 selvage williamsburg aesthetic. Paleo thundercats keytar, tousled literally banjo affogato heirloom bespoke leggings post-ironic. Tofu selfies swag hoodie, pabst ethical heirloom. Vinyl tumblr street art butcher mlkshk. Letterpress small batch keytar trust fund. Aesthetic vice mustache health goth dreamcatcher.</p>
      <h2>Beats</h2>
      <p>Food truck stumptown brunch, plaid kogi yr tousled squid art party. Aesthetic kogi try-hard asymmetrical humblebrag. Disrupt seitan raw denim intelligentsia selfies, migas poutine messenger bag. Microdosing bushwick salvia aesthetic, trust fund bitters locavore lo-fi shoreditch. Heirloom fingerstache stumptown, 3 wolf moon actually literally franzen everyday carry cliche church-key tote bag put a bird on it vegan pug truffaut. Heirloom cornhole small batch kombucha, tote bag asymmetrical jean shorts brooklyn DIY skateboard kale chips biodiesel. Whatever hoodie tousled, mlkshk typewriter shabby chic knausgaard twee occupy cold-pressed tote bag sustainable food truck VHS thundercats.</p>
      <h2>Battlestar Galactica</h2>
      <p>Shabby chic drinking vinegar blog, waistcoat kombucha direct trade tofu aesthetic mlkshk everyday carry meh bitters. Photo booth dreamcatcher chia flannel, single-origin coffee waistcoat chambray mustache truffaut hella. Banjo VHS readymade 8-bit actually. Vice narwhal pinterest intelligentsia, tacos cray chicharrones tilde dreamcatcher mlkshk kombucha distillery gochujang. Crucifix banjo mustache messenger bag cray migas. Gentrify occupy slow-carb banh mi hoodie ramps. Cardigan fixie hammock synth mumblecore lomo.</p>
    </section>
  
    <p>Content provided by the ever so charming <a href="http://www.hipsum.co">Hipsum</a>.</p>
  
  </main>
</div> <!-- /content -->

<!-- Footer -->
<footer id="footer">
  <div class="wrapper">
    <a href="https://andreasvirkus.github.io">
      <div class="logo">
        <div class="element logo-text pre-test" id="sdew_1" ><p>a</p></div> 
        <div class="element logo-text pre-test selected" id="sdew_2" ><p>J</p></div> 
        <div class="element logo-text pre-test" id="sdew_3" ><p>v</p></div>
      </div>
    </a>
  </div>
</footer>

```
CSS example1
```
#footer {
  width: 100%;
  background: rgba(0, 0, 0, 0.65);
  text-align: center;
  margin-left: auto;
  margin-right: auto;
}

#footer:hover #sdew_2 p {
  color: #e16036;
}

#footer-tag {
  color: #fff;
}

#footer-tag a {
  color: #fff;
}

#footer-tag a:hover {
  color: #e16036;
}

.logo {
  width: 150px;
  height: 100px;
  margin-left: auto;
  margin-right: auto;
  transform: translate(-15px, 0);
  color: #000;
  font-family: Josefin Slab, serif;
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  font-size: 64px;
}

.logo p {
  font-family: Josefin Slab, serif;
}

.logo:hover #sdew_2 p {
  color: #e16036;
}

.element {
  position: absolute;
  display: block;
  margin: 0;
  padding: 0;
  white-space: nowrap;
}

.element p {
  line-height: 1;
  margin: 0;
  padding: 0;
  text-rendering: optimizeLegibility;
  font-feature-settings: "kern";
}

#sdew_1 {
  font-size: 64px;
  color: #fff;
  top: 1px;
  left: 50px;
}

#sdew_2 {
  font-size: 64px;
  color: #fff;
  top: 30px;
  left: 77px;
}

#sdew_2 p {
  -webkit-transition: all 0.3s ease-in-out;
  -moz-transition: all 0.3s ease-in-out;
  -o-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
}

#sdew_3 {
  font-size: 64px;
  color: #fff;
  top: 40px;
  left: 92px;
}

```
HTML example2
```
<div class="wrap">
  <div class="container">
  <div class="box">
    <div class='smoke'>
    </div>
  </div>
</div>
</div> <!-- /content -->

<!-- Footer -->
<div id="footer">
  <div class="wrapper">
    <a href="https://andreasvirkus.github.io">
      <div class="logo">
        <div class="element logo-text pre-test" id="sdew_1" ><p>a</p></div> 
        <div class="element logo-text pre-test selected" id="sdew_2" ><p>J</p></div> 
        <div class="element logo-text pre-test" id="sdew_3" ><p>v</p></div>
      </div>
    </a>
  </div>
</div>

```
CSS example2
```
#footer {
  position: relative;
  background: rgba(0, 0, 0, 0.65);
  text-align: center;
  margin-left: auto;
  margin-right: auto;
}

#footer:hover #sdew_2 p {
  color: #e16036;
}

#footer-tag {
  color: #fff;
}

#footer-tag a {
  color: #fff;
}

#footer-tag a:hover {
  color: #e16036;
}

.logo {
  width: 150px;
  height: 100px;
  margin-left: auto;
  margin-right: auto;
  transform: translate(-15px, 0);
  color: #000;
  font-family: Josefin Slab, serif;
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  font-size: 64px;
}

.logo p {
  font-family: Josefin Slab, serif;
}

.logo:hover #sdew_2 p {
  color: #e16036;
}

.element {
  position: absolute;
  display: block;
  margin: 0;
  padding: 0;
  white-space: nowrap;
}

.element p {
  line-height: 1;
  margin: 0;
  padding: 0;
  text-rendering: optimizeLegibility;
  font-feature-settings: "kern";
}

#sdew_1 {
  font-size: 64px;
  color: #fff;
  top: 1px;
  left: 50px;
}

#sdew_2 {
  font-size: 64px;
  color: #fff;
  top: 30px;
  left: 77px;
}

#sdew_2 p {
  -webkit-transition: all 0.3s ease-in-out;
  -moz-transition: all 0.3s ease-in-out;
  -o-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
}

#sdew_3 {
  font-size: 64px;
  color: #fff;
  top: 40px;
  left: 92px;
}

```
---
# form tag
The form tag is used to create an HTML form for user input.

The form element can contain one or more of the following form elements:

input
textarea
button
select
option
optgroup
fieldset
label
output

example1
```
<form>
  <label for="foo">foo </label>
  <input type="text" id="foo" required>*
  <input id="saveFoo" type="submit" value="save">
</form>
<div>valid? <span id="valid"></span></div>
<div>u entered: <span id="output"></span></div>
<div>feedback: <span id="feedback"></span></div>

```
example2
```
<h3>iOS Keyboard: Bottom Right Button Variants</h3>

<!-- Keyboard w/ Return Button -->
<label for="username">Username</label>
<input id="username" class="input-returnKB" type="text" name="username2" value="" placeholder="Username Return" tabindex="1" autocorrect="off" autocapitalize="none">

<!-- Keyboard w/ GO Button -->
<form name="login" method="post" action="#">
  <label for="password">Password</label>
  <input id="password" type="password" name="password" value="" placeholder="Password GO" tabindex="2">
</form>

<!-- Description -->
<p>iOS Mobile Safari detects which keyboard to present a user by the structure of the HTML. There are two iOS Mobile Safari keyboard variants that have to do with the bottom right button. The button variations are "return" or "Go". "Go" is triggered by having a "form" tag with and defined "action".</p>

```
---












