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

# h1,h2,h3,h4,h5,h6 tag 

The h1 to h6 tags are used to define HTML headings.

h1 defines the most important heading. h6 defines the least important heading.

Note: Only use one h1 per page - this should represent the main heading/subject for the whole page. Also, do not skip heading levels - start with h1, then use h2, and so on.

example
```
<html>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>
<h4>This is heading 4</h4>
<h5>This is heading 5</h5>
<h6>This is heading 6</h6>

<p><b>Tip:</b> Use h1 to h6 elements only for headings. Do not use them just to make text bold or big. Use other tags for that.</p>

</body>
</html>

```
---
# head tag
The head element is a container for metadata (data about data) and is placed between the html tag and the body tag.

Metadata is data about the HTML document. Metadata is not displayed.

Metadata typically define the document title, character set, styles, scripts, and other meta information.

The following elements can go inside the head element:

title (required in every HTML document),
style,
base,
link,
meta,
script,
noscript,
---
# header tag
The header element represents a container for introductory content or a set of navigational links.

A header element typically contains:

one or more heading elements (h1 - h6)
logo or icon
authorship information

HTML example1
```
<!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">

        <!--=============== BOXICONS ===============-->
        <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/boxicons@latest/css/boxicons.min.css">

        <!--=============== CSS ===============-->
        <link rel="stylesheet" href="assets/css/styles.css">

        <title>Responsive bottom navigation</title>
    </head>
    <body>
        <!--=============== HEADER ===============-->
        <header class="header" id="header">
            <nav class="nav container">
                <a href="#" class="nav__logo">Marlon</a>

                <div class="nav__menu" id="nav-menu">
                    <ul class="nav__list">
                        <li class="nav__item">
                            <a href="#home" class="nav__link active-link">
                                <i class='bx bx-home-alt nav__icon'></i>
                                <span class="nav__name">Home</span>
                            </a>
                        </li>
                        
                        <li class="nav__item">
                            <a href="#about" class="nav__link">
                                <i class='bx bx-user nav__icon'></i>
                                <span class="nav__name">About</span>
                            </a>
                        </li>

                        <li class="nav__item">
                            <a href="#skills" class="nav__link">
                                <i class='bx bx-book-alt nav__icon'></i>
                                <span class="nav__name">Skills</span>
                            </a>
                        </li>

                        <li class="nav__item">
                            <a href="#portfolio" class="nav__link">
                                <i class='bx bx-briefcase-alt nav__icon'></i>
                                <span class="nav__name">Portfolio</span>
                            </a>
                        </li>

                        <li class="nav__item">
                            <a href="#contactme" class="nav__link">
                                <i class='bx bx-message-square-detail nav__icon'></i>
                                <span class="nav__name">Contactme</span>
                            </a>
                        </li>
                    </ul>
                </div>

                <img src="assets/img/perfil.png" alt="" class="nav__img">
            </nav>
        </header>

        <main>
            <!--=============== HOME ===============-->
            <section class="container section section__height" id="home">
                <h2 class="section__title">Home</h2>
            </section>

            <!--=============== ABOUT ===============-->
            <section class="container section section__height" id="about">
                <h2 class="section__title">About</h2>
            </section>

            <!--=============== SKILLS ===============-->
            <section class="container section section__height" id="skills">
                <h2 class="section__title">Skills</h2>
            </section>

            <!--=============== PORTFOLIO ===============-->
            <section class="container section section__height" id="portfolio">
                <h2 class="section__title">Portfolio</h2>
            </section>

            <!--=============== CONTACTME ===============-->
            <section class="container section section__height" id="contactme">
                <h2 class="section__title">Contactme</h2>
            </section>
        </main>
        

        <!--=============== MAIN JS ===============-->
        <script src="assets/js/main.js"></script>
    </body>
</html>
```
example2
```
<h2>Examples of Using the &lt;header&gt; Tag</h2>

<div class="examples">
  <div class="unstyled">
    <h3>Default Appearance</h3>
    <header>
      <h4>Choose a Category</h4>
      <nav>
        <ul>
          <li><a href="/html.php">HTML</a>
            <li><a href="/css.php">CSS</a>
              <li><a href="/sass.php">Sass</a>
        </ul>
      </nav>
    </header>
  </div>
  <div class="styled">
    <h3>Styled Using CSS</h3>
    <header>
      <h4>Choose a Category</h4>
      <nav>
        <ul>
          <li><a href="/html.php">HTML</a>
            <li><a href="/css.php">CSS</a>
              <li><a href="/sass.php">Sass</a>
        </ul>
      </nav>
    </header>
  </div>
</div>

```
CSS example2
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

.examples .styled header {
  font-variant: small-caps;
  font-size: larger;
}

.examples .styled header ul{
  list-style: none;
  margin-left: 0;
  padding-left: 0;
}

.examples .styled header ul li{
  margin-right: 20px;
  background: black;
  padding: 5px;
  border-radius: 4px;
  display: inline-block;
  
}

.examples .styled header ul li a{
  text-decoration: none;
  color: yellow;
  cursor: pointer;
  font-variant: none;
}

```
---
# hr tag
The hr tag defines a thematic break in an HTML page (e.g. a shift of topic).

The hr element is most often displayed as a horizontal rule that is used to separate content (or define a change) in an HTML page.

example1
```
<hr class="hr-1">
<hr class="hr-2">
<hr class="hr-3">
<hr class="hr-4">
<hr class="hr-5">
<hr class="hr-6">
<hr class="hr-7">
<hr class="hr-8">
<hr class="hr-9">
<hr class="hr-10">
<hr class="hr-11">
<hr class="hr-12">
<hr class="hr-13">
<hr class="hr-14">
<hr class="hr-15">
<hr class="hr-16">
<hr class="hr-17">
<hr class="hr-18">
<hr class="hr-19">

```
CSS example1
```
hr {
  background-color: #fff;
  padding: 0;
  margin: 80px;
}

hr.hr-1 {
  border: 0;
  height: 1px;
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0));
}

hr.hr-2 {
  border: 0;
  border-bottom: 2px dashed #eee;
  background: #999;
}

hr.hr-3 {
  border: 0;
  height: 0;
  border-top: 1px solid #8c8c8c;
}

hr.hr-4 {
  padding: 0;
  border: none;
  border-top: medium double #8c8c8c;
  color: #8c8c8c;
  text-align: center;
}

hr.hr-4:after {
  content: "§";
  display: inline-block;
  position: relative;
  top: -0.7em;
  font-size: 1.5em;
  padding: 0 0.25em;
  background: #fff;
}

hr.hr-5 {
  border: 0;
  border-top: 3px double #8c8c8c;
}

hr.hr-6 {
  border: 0;
  border-top: 2px dotted #8c8c8c;
}

hr.line-7 {
  border: 0;
  background-color: #fff;
  border-top: 1px dashed #8c8c8c;
}

hr.hr-8 {
  border: 0;
  background-color: #fff;
  border-top: 2px dotted #8c8c8c;
}

hr.hr-9 {
  border: 0;
  border-top: 1px solid #8c8c8c;
  border-bottom: 1px solid #fff;
}

hr.hr-10 {
  border: 0;
  border-top: 1px solid #8c8c8c;
  border-bottom: 1px solid #fff;
}

hr.hr-10:after {
  content: '';
  display: block;
  margin-top: 2px;
  border-top: 1px solid #8c8c8c;
  border-bottom: 1px solid #fff;
}

hr.hr-11 {
  border: 0;
  border-top: 1px dashed #8c8c8c;
  border-bottom: 1px dashed #fff;
}

hr.hr-12 {
  border: 0;
  border-top: 1px dotted #8c8c8c;
  border-bottom: 1px dotted #fff;
}

hr.hr-13 {
  height: 10px;
  border: 0;
  box-shadow: 0 10px 10px -10px #8c8c8c inset;
}

hr.hr-14 {
  border: 0;
  height: 1px;
  background-image: -webkit-linear-gradient(left, #f0f0f0, #8c8c8c, #f0f0f0);
  background-image: -moz-linear-gradient(left, #f0f0f0, #8c8c8c, #f0f0f0);
  background-image: -ms-linear-gradient(left, #f0f0f0, #8c8c8c, #f0f0f0);
  background-image: -o-linear-gradient(left, #f0f0f0, #8c8c8c, #f0f0f0);
}

hr.hr-15 {
  border: 0;
  border-top: 4px double #8c8c8c;
  text-align: center;
}

hr.hr-15:after {
  content: '\2665';
  display: inline-block;
  position: relative;
  top: -15px;
  padding: 0 10px;
  background: #fff;
  color: #8c8c8c;
  font-size: 18px;
}

hr.hr-16 {
  border: 0;
  border-top: 1px dashed #8c8c8c;
  text-align: center;
}

hr.hr-16:after {
  content: '\002702';
  display: inline-block;
  position: relative;
  top: -13px;
  padding: 0 3px;
  background: #fff;
  color: #8c8c8c;
  font-size: 18px;
}

hr.hr-17 {
  border: 0;
  height: 0;
  box-shadow: 0 0 10px 1px black;
}

hr.hr-17:after {
  content: "\00a0";
}

hr.hr-18 {
  background-color: #fff;
  height: 30px;
  border: 1px solid #8c8c8c;
  border-radius: 20px;
}

hr.hr-18:before {
  display: block;
  content: "";
  height: 30px;
  margin-top: -31px;
  border: 0 solid #8c8c8c;
  border-bottom-width: 1px;
  border-radius: 20px;
}

.hr-19 {
  border: none;
  height: 10px;
  background: linear-gradient(-135deg, #fff 5px, transparent 0) 0 5px, linear-gradient(135deg, #fff 5px, #8c8c8c 0) 0 5px;
  background-color: #fff;
  background-position: left bottom;
  background-repeat: repeat-x;
  background-size: 10px 10px;
}

```
HTML example2
```
<html>
<body>

<h1>The Main Languages of the Web</h1>

<p>HTML is the standard markup language for creating Web pages. HTML describes the structure of a Web page, and consists of a series of elements. HTML elements tell the browser how to display the content.</p>

<hr>

<p>CSS is a language that describes how HTML elements are to be displayed on screen, paper, or in other media. CSS saves a lot of work, because it can control the layout of multiple web pages all at once.</p>

<hr>

<p>JavaScript is the programming language of HTML and the Web. JavaScript can change HTML content and attribute values. JavaScript can change CSS. JavaScript can hide and show HTML elements, and more.</p>

</body>
</html>

```
---
# html tag

The html tag represents the root of an HTML document.

The html tag is the container for all other HTML elements (except for the <!DOCTYPE> tag).
---
# italic tag

The i tag defines a part of text in an alternate voice or mood. The content inside is typically displayed in italic.

The i tag is often used to indicate a technical term, a phrase from another language, a thought, a ship name, etc.

Use the i element only when there is not a more appropriate semantic element, such as:

em (emphasized text)
strong (important text)
mark (marked/highlighted text)
cite (the title of a work)
dfn (a definition term)

example
```
<html>
<body>

<h1>The i element</h1>

<p><i>Lorem ipsum</i> is the most popular filler text in history.</p>

<p>The <i>RMS Titanic</i>, a luxury steamship, sank on April 15, 1912 after striking an iceberg.</p>

</body>
</html>

```
---

# img tag
The img tag is used to embed an image in an HTML page.

Images are not technically inserted into a web page; images are linked to web pages. The img tag creates a holding space for the referenced image.

The img tag has two required attributes:

src - Specifies the path to the image
alt - Specifies an alternate text for the image, if the image for some reason cannot be displayed

example1 HTML
```
<div class="cover">
  <img src="https://www.google.fr/images/srpr/logo11w.png" class="cover" />
</div>

```
example1 CSS
```
div.cover {
  position: fixed; 
  top: -50%; 
  left: -50%; 
  width: 200%; 
  height: 200%;
}
img.cover {
  position: absolute; 
  top: 0; 
  left: 0; 
  right: 0; 
  bottom: 0; 
  margin: auto; 
  min-width: 50%;
  min-height: 50%;
  overflow-x: hidden;
}

```
example2 HTML
```
<div class="wrapper">
  
  <img src="https://i.kinja-img.com/gawker-media/image/upload/gd8ljenaeahpn0wslmlz.jpg" class="image--cover">
  
  <img src="http://imgc.allpostersimages.com/images/P-473-488-90/68/6896/2GOJ100Z/posters/despicable-me-2-minions-movie-poster.jpg" alt="" class="image--cover" />
  
  <img src="http://static.eharmony.com/blog/wp-content/uploads/2010/04/eHarmony-Blog-profile-picture.jpg" alt="" class="image--cover" />
  
  <img src="https://i2.cdn.turner.com/cnnnext/dam/assets/140926165711-john-sutter-profile-image-large-169.jpg" alt="" class="image--cover" />
</div>

```
CSS example2
```
.wrapper {
  padding: 100px;
}

.image--cover {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  margin: 20px;

  object-fit: cover;
  object-position: center right;
}

```
---

# input tag
The input tag specifies an input field where the user can enter data.

The input element is the most important form element.

The input element can be displayed in several ways, depending on the type attribute.

The different input types are as follows:

input type="button"
input type="checkbox"
input type="color"
input type="date"
input type="datetime-local"
input type="email"
input type="file"
input type="hidden"
input type="image"
input type="month"
input type="number"
input type="password"
input type="radio"
input type="range"
input type="reset"
input type="search"
input type="submit"
input type="tel"
input type="text" (default value)
input type="time"
input type="url"
input type="week"
Look at the type attribute to see examples for each input type!

HTML example1
```
<form>
  <div>
  <p>
    <label>
      text<br>
    <input type="text">
    </label>
  </p>
  <p>
    <label>
      password<br>
    <input type="password">
    </label>
  </p>
  <p>
    <label>
      number<br>
    <input type="number">
    </label>
  </p>
  <p>
    <label>
      email<br>
    <input type="email">
    </label>
  </p>
  <p>
    <label>
      url<br>
    <input type="url">
    </label>
  </p>
  <p>
    <label>
      tel<br>
    <input type="tel">
    </label>
  </p>
  <p>
    <label>
      search<br>
    <input type="search">
    </label>
  </p>
  <p>
    <label>
      textarea<br>
      <textarea></textarea>
    </label>
  </p>
  <p>
    <label>
      date<br>
    <input type="date">
    </label>
  </p>
  <p>
    <label>
      datetime<br>
    <input type="datetime">
    </label>
  </p>
  <p>
    <label>
      datetime-local<br>
    <input type="datetime-local">
    </label>
  </p>
  <p>
    <label>
      month<br>
    <input type="month">
    </label>
  </p>
  <p>
    <label>
      week<br>
    <input type="week">
    </label>
  </p>
  <p>
    <label>
      time<br>
    <input type="time">
    </label>
  </p>
  <p>
    <label>
      select<br>
      <select>
        <optgroup label="optgroup">
          <option>option 1</option>
          <option>option 2</option>
          <option>option 3</option>
        </optgroup>
      </select>
    </label>
  </p>
  <p>
    <label>
      select (multiple attr)<br>
      <select multiple>
        <optgroup label="optgroup">
          <option>option 1</option>
          <option>option 2</option>
          <option>option 3</option>
        </optgroup>
      </select>
    </label>
  </p>
  <p>
    <label>
      select (size attr)<br>
      <select size="4">
        <optgroup label="optgroup">
          <option>option 1</option>
          <option>option 2</option>
          <option>option 3</option>
        </optgroup>
      </select>
    </label>
  </p>
  <p>
    <label>
      datalist<br>
      <input list="datalist">
      <datalist id="datalist">
        <option value="option 1">
        <option value="option 2">
        <option value="option 3">
      </datalist>
    </label>
  </p>
  <p>
    <label>
      keygen<br>
      <keygen>
    </label>
  </p>
  <p>
    <label>
      output<br>
      <output>123</output>
    </label>
  </p>
  <p>
    <label>
      radio<br>
    <input type="radio">
    </label>
  </p>
  <p>
    <label>
      checkbox<br>
    <input type="checkbox">
    </label>
  </p>
  <p>
    <label>
      color<br>
    <input type="color">
    </label>
  </p>
  <p>
    <label>
      range<br>
    <input type="range">
    </label>
  </p>
  <p>
    <label>
      file<br>
    <input type="file">
    </label>
  </p>
  <p>
    <label>
      submit<br>
    <input type="submit">
    </label>
  </p>
  <p>
    <label>
      reset<br>
    <input type="reset">
    </label>
  </p>
  <p>
    <label>
      button (input tag)<br>
    <input type="button" value="Button">
    </label>
  </p>
  <p>
    <label>
      button (button tag)<br>
      <button>Button</button>
    </label>
  </p>
  </div>
  <fieldset>
    <legend>legend</legend>
    fieldset
  </fieldset>
</form>

```
CSS example1
```
html, body {
  margin:0;
  padding:0;
}

form div {
  display:flex;
  flex-wrap:wrap;
}

form p {
  margin:1em;
  padding:1em;
}

form label {
  color:#999;
  font-family:sans-serif;
}

fieldset {
  margin:2em;
}

```
HTML example2
```
<div class="container">
  <div class="radio-tile-group">
    <div class="input-container">
      <input id="walk" class="radio-button" type="radio" name="radio" />
      <div class="radio-tile">
        <div class="icon walk-icon">
          <svg fill="#000000" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
            <path d="M0 0h24v24H0z" fill="none"/>
            <path d="M13.5 5.5c1.1 0 2-.9 2-2s-.9-2-2-2-2 .9-2 2 .9 2 2 2zM9.8 8.9L7 23h2.1l1.8-8 2.1 2v6h2v-7.5l-2.1-2 .6-3C14.8 12 16.8 13 19 13v-2c-1.9 0-3.5-1-4.3-2.4l-1-1.6c-.4-.6-1-1-1.7-1-.3 0-.5.1-.8.1L6 8.3V13h2V9.6l1.8-.7"/>
          </svg>
        </div>
        <label for="walk" class="radio-tile-label">Walk</label>
      </div>
    </div>

    <div class="input-container">
      <input id="bike" class="radio-button" type="radio" name="radio" />
      <div class="radio-tile">
        <div class="icon bike-icon">
          <svg fill="#000000" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
            <path d="M0 0h24v24H0z" fill="none"/>
            <path d="M15.5 5.5c1.1 0 2-.9 2-2s-.9-2-2-2-2 .9-2 2 .9 2 2 2zM5 12c-2.8 0-5 2.2-5 5s2.2 5 5 5 5-2.2 5-5-2.2-5-5-5zm0 8.5c-1.9 0-3.5-1.6-3.5-3.5s1.6-3.5 3.5-3.5 3.5 1.6 3.5 3.5-1.6 3.5-3.5 3.5zm5.8-10l2.4-2.4.8.8c1.3 1.3 3 2.1 5.1 2.1V9c-1.5 0-2.7-.6-3.6-1.5l-1.9-1.9c-.5-.4-1-.6-1.6-.6s-1.1.2-1.4.6L7.8 8.4c-.4.4-.6.9-.6 1.4 0 .6.2 1.1.6 1.4L11 14v5h2v-6.2l-2.2-2.3zM19 12c-2.8 0-5 2.2-5 5s2.2 5 5 5 5-2.2 5-5-2.2-5-5-5zm0 8.5c-1.9 0-3.5-1.6-3.5-3.5s1.6-3.5 3.5-3.5 3.5 1.6 3.5 3.5-1.6 3.5-3.5 3.5z"/>
          </svg>
        </div>
        <label for="bike" class="radio-tile-label">Bike</label>
      </div>
    </div>

    <div class="input-container">
      <input id="drive" class="radio-button" type="radio" name="radio" />
      <div class="radio-tile">
        <div class="icon car-icon">
          <svg fill="#000000" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
            <path d="M18.92 6.01C18.72 5.42 18.16 5 17.5 5h-11c-.66 0-1.21.42-1.42 1.01L3 12v8c0 .55.45 1 1 1h1c.55 0 1-.45 1-1v-1h12v1c0 .55.45 1 1 1h1c.55 0 1-.45 1-1v-8l-2.08-5.99zM6.5 16c-.83 0-1.5-.67-1.5-1.5S5.67 13 6.5 13s1.5.67 1.5 1.5S7.33 16 6.5 16zm11 0c-.83 0-1.5-.67-1.5-1.5s.67-1.5 1.5-1.5 1.5.67 1.5 1.5-.67 1.5-1.5 1.5zM5 11l1.5-4.5h11L19 11H5z"/>
            <path d="M0 0h24v24H0z" fill="none"/>
          </svg>
        </div>
        <label for="drive" class="radio-tile-label">Drive</label>
      </div>
    </div>

    <div class="input-container">
      <input id="fly" class="radio-button" type="radio" name="radio" />
      <div class="radio-tile">
        <div class="icon fly-icon">
          <svg fill="#000000" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
            <path d="M10.18 9"/>
            <path d="M21 16v-2l-8-5V3.5c0-.83-.67-1.5-1.5-1.5S10 2.67 10 3.5V9l-8 5v2l8-2.5V19l-2 1.5V22l3.5-1 3.5 1v-1.5L13 19v-5.5l8 2.5z"/>
            <path d="M0 0h24v24H0z" fill="none"/>
          </svg>
        </div>
        <label for="fly" class="radio-tile-label">Fly</label>
      </div>
    </div>
  </div>
</div>

```
CSS example2
```
* {
  box-sizing: border-box;
  font-family: 'Helvetica Neue', sans-serif;
}

body {
  background-color: black;
}

$primary-color: #079ad9;

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.radio-tile-group {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;

  //set dimensions for invisible container
  .input-container {
    position: relative;
    height:  7rem;
    width:  7rem;
    margin: 0.5rem;

    //make actual radio input invisible
    // + stretch to fill container
    .radio-button {
      opacity: 0;
      position: absolute;
      top: 0;
      left: 0;
      height: 100%;
      width: 100%;
      margin: 0;
      cursor: pointer;
    }

    //default tile styles
    .radio-tile {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      width: 100%;
      height: 100%;
      border: 2px solid $primary-color;
      border-radius: 5px;
      padding: 1rem;
      transition: transform 300ms ease;
    }
    .icon svg {
      fill: $primary-color;
      width: 3rem;
      height: 3rem;
    }
    .radio-tile-label {
      text-align: center;
      font-size: 0.75rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 1px;
      color: $primary-color;
    }

    //active tile styles
    .radio-button:checked + .radio-tile {
      background-color: $primary-color;
      border: 2px solid $primary-color;
      color: white;
      transform: scale(1.1, 1.1);
      
      .icon svg {
        fill: white;
        background-color: $primary-color;
      }
      .radio-tile-label {
        color: white;
        background-color: $primary-color;
      }
    }
  }
}

```
---
# ins tag
The ins tag defines a text that has been inserted into a document. Browsers will usually underline inserted text.

example1
```
<section class="style-1">
  <h2 id="style-name">School Essay</h2>
  <ol id="quotes">
    <li><p>The early bird catches <del>the worm</del><ins>less sleep</ins>.</p></li>
    <li><p>The best things in life are <del>free</del><ins>extremely expensive</ins>.</p></li>
    <li><p>Shoot for the moon. Even if you miss, you'll <del>land among the stars</del><ins>suffocate in outer space and die</ins>.</p></li>
    <li><p><del>Everything</del><ins>Nothing</ins> is going to be fine.</p></li>
    <li><p>Big girls don't <del>cry</del><ins>submit to people telling them what to do</ins>.</p></li>
  </ol>
</section>


<button data-style="style-1" data-title="School Essay">Style 1</button>
<button data-style="style-2"data-title="Update on Hover">Style 2</button>

```
Example2
```
<html>
<body>

<h1>The ins element</h1>

<p>My favorite color is <del>blue</del> <ins>red</ins>!</p>

</body>
</html>

```
---
# kbd tag
The kbd tag is used to define keyboard input. The content inside is displayed in the browser's default monospace font.

example1
```
<html>
<body>

<h1>The kbd element</h1>

<p>Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy text (Windows).</p>

<p>Press <kbd>Cmd</kbd> + <kbd>C</kbd> to copy text (Mac OS).</p>

</body>
</html>

```
example2
```
<p>To paste copied text content stripped of formatting, use <kbd>⌘</kbd>+<kbd>Opt</kbd>+<kbd>Shift</kbd>+<kbd>V</kbd>.</p>

```
# label tag
The label tag defines a label for several elements:

input type="checkbox"

input type="color"

input type="date"

input type="datetime-local"

input type="email"

input type="file"

input type="month"

input type="number"

input type="password"

input type="radio"

input type="range"

input type="search"

input type="tel"

input type="text"

input type="time"

input type="url"

input type="week"

meter

progress

select

textarea

 example
```
<html>
<body>

<h1>The label element</h1>

<p>Click on one of the text labels to toggle the related radio button:</p>

<form action="/action_page.php">
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label><br><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>

```
---
# legend tag
The legend tag defines a caption for the fieldset element.

example
```
<html>
<body>

<h1>The legend element</h1>

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
---

# LI tag
The li tag defines a list item.

The li tag is used inside ordered lists(ol), unordered lists (ul), and in menu lists menu.

In ul and menu, the list items will usually be displayed with bullet points.

In ol, the list items will usually be displayed with numbers or letters.

example1
```
<ul>
  <li>One lorem ipsum dolor sit amet</li><!--
  --><li>Two</li><!--
  --><li>Three</li><!--
  --><li><p>Four</p></li><!--
  --><li><img src="http://placehold.it/50/50" /></li>
</ul>

```
example2

HTML
```
<ul>
 <li class="link"><a href="#">Alpha Link</a></li>
 <li class="link"><a href="#">Beta Link</a></li>
 <li class="link"><a href="#">Charlie Link</a></li>
 <li class="link"><a href="#">Delta Link</a></li>
 <li class="link"><a href="#">Echo Link</a></li>
 <li class="link"><a href="#">Foxtrot Link</a></li>
 <li class="link"><a href="#">Golf Link</a></li>
</ul>

```
CSS example2
```
.link{
  text-decoration: none;
    border-color: #3AC162;
	  background-color: #5FCF80;
    border-style: solid;
    border-width: 0px 0px 3px;
    box-shadow: 0 -1px 0 rgba(255, 255, 255, 0.1) inset;
    color: #FFFFFF;	   
    border-radius: 6px;
    cursor: pointer;
    display: inline-block;
    font-style: normal;
    overflow: hidden;
    text-align: center;
    text-decoration: none;
    text-overflow: ellipsis;
    transition: all 200ms ease-in-out 0s;
    white-space: nowrap;	
    font-family: "Gotham Rounded A","Gotham Rounded B",Helvetica,Arial,sans-serif;
    font-weight: 700;	
    padding: 19px 39px 18px;
  a{
    text-decoration: none;
    font-size: 18px;
    color: white;
  }
  &.active{
    background-color: #ED5A5A;
    border-color: #EA4343;
  }
}

```
---
# link tag
The link tag defines the relationship between the current document and an external resource.

The link tag is most often used to link to external style sheets or to add a favicon to your website.

The link element is an empty element, it contains attributes only.

example1 HTML
```
<div id="app">
  <transition mode="out-in">
    <router-view :key="$route.path"></router-view>
  </transition>
  <ul>
    <router-link tag="li" to="/" exact><a>Home</a></router-link>
    <router-link tag="li" to="/page/1"><a>Page 1</a></router-link>
    <router-link tag="li" to="/page/2"><a>Page 2</a></router-link>
    <router-link tag="li" to="/user/mimi"><a>Mimi</a></router-link>
    <router-link tag="li" to="/user/mintuno"><a>Mintuno</a></router-link>
  </ul>
</div>

```
CSS example1
```
body {
  font-family: sans-serif;
}

a {
  color: inherit;
  text-decoration: none;
}

.router-link-active {
  color: cornflowerblue;
  font-weight: bold;
}

.box {
  padding: 1em;
  border: 1px solid #333;
}

.home {
  color: #900;
  border-color: #900;
  background-color: #fcc;
}

.page {
  color: #090;
  border-color: #090;
  background-color: #cfc;
}

.user {
  color: #009;
  border-color: #009;
  background-color: #ccf;
}

.v-enter, .v-leave-to {
  opacity: 0;
}

.v-enter-active, .v-leave-active{
  transition: all 250ms ease-in;
}

```

HTML example2
```
<h1>Header</h1>
<p>Lorem ipsum&hellip;</p>
<p>More information can be found at <a href="http://kurtzenisek.com/p/smart-web-banner/" target="_blank">http://kzeni.com/p/smart-web-banner/</a>
<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js"></script>
<script type="text/javascript" src="http://kurtzenisek.com/p/smart-web-banner/jQuery.smartWebBanner.js"></script>

```
---

# main tag
The main tag specifies the main content of a document.

The content inside the main element should be unique to the document. It should not contain any content that is repeated across documents such as sidebars, navigation links, copyright information, site logos, and search forms.

HTML Example1
```
<body>
  <nav id="toc">
  </nav>
  <main>
    <h1>New Horizons</h1>
    <p>
      Live life at your own pace as you garden, fish, decorate, hunt for bugs and fossils, get to know the animal residents, and more. The time of day and seasons match real life, so something is happening on your island whether you’re there or not.
    </p>
    <p>Oh--just watch out for those shifty racoons.</p>
    <h2>Tools</h2>
    <p>New Horizons has all sorts of tools that you can use to your disposal!</p>
    <h3>Shovel</h3>
    <p>This tool's versatility knows no bounds! Hole digging, rock smacking, tree uprooting goodness!</p>
    <h3>Bug Net</h3>
    <p>Catch some bugs--if you are into that kind of thing.</p>
    <h3>Slingshot</h3>
    <p>Make presents fall from the sky! Just watch out for the river!</p>
    <h3>Fishing Rod</h3>
    <p>After all that shovel work its nice to take a load of, craft a nice coconut juice, and fish.</p>
    <h3>Ladder</h3>
    <p>For those annoying cliffs.</p>
    <h3>Axe</h3>
    <p>For choppin' trees--just watch out for them bees!</p>
    <h3>Vaulting Pole</h3>
    <p>For those like me, that are too poor to afford a bridge.</p>
    <h3>Watering Can</h3>
    <p>Those flowers won't crossbreed themselves.</p>
    <h2>Flower Crossbreeding</h2>
    <h3>Lilies</h3>
    <ul>
      <li>Red + Red = Black</li>
      <li>Yellow + Red = Orange</li>
      <li>Red + White = Pink</li>
    </ul>
    <h3>Roses</h3>
    <ul>
      <li>Red + Red = Black</li>
      <li>Red + White = Pink</li>
      <li>Yellow + Red = Orange</li>
      <li>White + White = Purple</li>
    </ul>
    <h3>Mums</h3>
    <ul>
      <li>White + Red = Pink</li>
      <li>White + White = Purple</li>
      <li>Purple + Purple = Green</li>
    </ul>
    <h3>Pansies</h3>
    <ul>
      <li>Red + Red = Purple</li>
      <li>White + White = Blue</li>
      <li>Yellow + Red = Orange</li>
      <li>Blue + Blue = Purple</li>
      <li>Red + Red = Purple</li>
    </ul>
    <h3>Windflower</h3>
    <ul>
      <li>Orange + Red = Pink</li>
      <li>Orange + White = Blue</li>
      <li>White + White = Blue</li>
      <li>Blue + Pink = Purple</li>
      <li>Blue + Blue = Purple</li>
    </ul>
    <h3>Hyacinths</h3>
    <ul>
      <li>Red + White = Pink</li>
      <li>White + White = Blue</li>
      <li>Red + Yellow = Orange</li>
      <li>Blue + Blue = Purple</li>
    </ul>
    <h3>Cosmos</h3>
    <ul>
      <li>Yellow + Red = Orange</li>
      <li>Red + White = Pink</li>
      <li>Red + Red = Black</li>
    </ul>
    <h3>Tulips</h3>
    <ul>
      <li>Red + Red = Black</li>
      <li>Red + Yellow = Orange</li>
      <li>Red + White = Pink</li>
      <li>Black + Black = Purple</li>
    </ul>
  </main>
</body>

```
CSS example1
```
body {
  display: flex;
  flex-flow: space-between;
  height: 100vh;
  font-family: "Rubik";
  margin: 0;
  color: #333344;
  line-height: 1.53em;
  font-size: 1.2rem;
  background-color: #efeeff;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Rubik Mono One";
  font-weight: 300;
  margin-top: 3rem;
  color: #484866;
}

main {
  flex: 3 3 100%;
  overflow: auto;
  padding: 2rem 3rem;
}

nav {
  flex: 1 1 300px;
  background-color: #333344;
  min-width: 240px;
  paddings: 1rem;
  overflow-y: auto;
}

h1,
h2,
p {
  max-width: 700px;
}

a {
  color: #eeeeff;
  text-decoration: none;
}

.active {
  color: #ff8888;
  font-weight: bold;
}

ul {
  list-style: none;
  padding-left: 1.25rem;
}

ul li::before {
  content: "\2022";
  color: #eeeeff;
  font-weight: bold;
  display: inline-block;
  width: 1em;
  margin-left: -1em;
}

```
example2
```
<html>
<body>

<h1>The main element</h1>

<main>
  <h1>Most Popular Browsers</h1>
  <p>Chrome, Firefox, and Edge are the most used browsers today.</p>

  <article>
    <h2>Google Chrome</h2>
    <p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!</p>
  </article>

  <article>
    <h2>Mozilla Firefox</h2>
    <p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
  </article>

  <article>
    <h2>Microsoft Edge</h2>
    <p>Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.</p>
  </article>
</main>

</body>
</html>

```
---
# map tag
The map tag is used to define an image map. An image map is an image with clickable areas.

The required name attribute of the map element is associated with the img's usemap attribute and creates a relationship between the image and the map.

example
```
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
---
# mark tag

The mark tag defines text that should be marked or highlighted.

example
```
<html>
<body>

<h1>The mark element</h1>

<p>Do not forget to buy <mark>milk</mark> today.</p>

</body>
</html>

```
---
The meta tag defines metadata about an HTML document. Metadata is data (information) about data.

meta tags always go inside the head element, and are typically used to specify character set, page description, keywords, author of the document, and viewport settings.

Metadata will not be displayed on the page, but is machine parsable.

Metadata is used by browsers (how to display content or reload page), search engines (keywords), and other web services.

There is a method to let web designers take control over the viewport (the user's visible area of a web page), through the meta tag (See "Setting The Viewport" example below).

Example1

HTML
```
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
</head>
<body>
<!-- ---------------- -->
  <main class="main">
    
    <section class="section section--pos">
      <div class="iphone"><span class="iphone__txt">X</span></div>
      <h1 class="heading heading--1">
        <span style="font-size: .5em">Tutorial</span><br>
        Designing for the Notch
      </h1>
      <p style="text-align: center;">
        <i>Note: As of iOS 11.2, "const()" has been removed in favor of the standardized "env()".</i>
      </p>
    </section>
    <section class="section section--neg">
      <h2 class="heading heading--2">Changing the viewport meta tag</h2>
      <div class="box">
        <p class="paragraph">
          First of all you need to add a declaration to your meta viewport content attribute:
        </p>
        <code class="code">
          <span class="color--opacity-0-5">&lt;meta name="viewport" content="width=device-width, initial-scale=1.0, </span>viewport-fit=cover<span class="color--opacity-0-5">"&gt;</span>
        </code>
      </div>
    </section>
    <section class="section section--pos">
      <h2 class="heading heading--2">Changing the CSS</h2>
      <div class="grid grid--split-33 grid--gut-20">
        
        <div class="grid__item">
          <div class="box">
            <h3 class="heading heading--3">The CSS</h3>
            <p class="paragraph">
              Since the code above will cause the painted area to fill the entire width of an iPhone X – we need to push the padding according to the device's "safe area".<br>
              You do this using the <del>constant [ const() ]</del> <ins>environment variable [ env() ]</ins>...<br>
              For areas that does not already require padding you can add:
            </p>
            <code class="code">
              <pre class="pre"><span class="color--opacity-0-5">.elem {</span>
  padding-right: env(safe-area-inset-right);
  padding-left: env(safe-area-inset-left);
<span class="color--opacity-0-5">}</span></pre>
            </code>
          </div>
        </div>
        
        <div class="grid__item">
          <div class="box">
            <h3 class="heading heading--3">The falback</h3>
            <p class="paragraph">
              Also, don't forget to define the fallback values for the devices that don't support <del>constant()</del> <ins>env()</ins> – in the case of no padding:
            </p>
            <code class="code">
              <pre class="pre"><span class="color--opacity-0-5">.elem {</span>
  padding-right: 0;
  padding-right: env(safe-area-inset-right);
  padding-left: 0;
  padding-left: env(safe-area-inset-left);
<span class="color--opacity-0-5">}</span></pre>
            </code>
          </div>
        </div>
        
        <div class="grid__item">
          <div class="box">
            <h3 class="heading heading--3">The combination</h3>
            <p class="paragraph">
              In case your element normally has 20 px padding, you can use the built-in function calc() to calculate the correct combined padding:
            </p>
            <code class="code">
              <pre class="pre"><span class="color--opacity-0-5">.elem {</span>
  padding-right: 20px;
  padding-right: calc( 20px + env(safe-area-inset-right) );
  padding-left: 20px;
  padding-left: calc( 20px + env(safe-area-inset-left) );
<span class="color--opacity-0-5">}</span></pre>
            </code>
          </div>
        
      </div>
    </section>
    
  </main>
  
<!-- ---------------- -->
</body>
</html>


```
CSS 

example1
```
@mixin pad() {
  
}

$col_a: #fb3;
$col_b: #333;

*, *::before, *::after {
  box-sizing: border-box;
}
html {
  font-size: 16px;
  line-height: 1.5;
  color: rgba(0,0,0,0.9);
}
body {
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  background: #333;
}


.main {
  display: flex;
  flex-flow: row wrap;
  justify-content: flex-start;
  align-items: flex-start;
  align-content: flex-start;
}
.section {
  // Notch styling
  padding: 50px 20px;
  padding-right: calc(20px + constant(safe-area-inset-right));
  padding-left: calc(20px + constant(safe-area-inset-left));
  
  // Arbitrary styling
  width: 100%;
  color: #333;
  
  &--pos {
    background: $col_a;
    color: $col_b;
  }
  &--neg {
    background: $col_b;
    color: $col_a;
  }
}
.heading {
  text-align: center;
  &--1 {
    margin: 0.25em 0;
    font-size: 2em;
    color: $col_b;
  }
}
.grid {
  display: flex;
  flex-flow: row wrap;
  justify-content: flex-start;
  align-items: stretch;
  align-content: flex-start;

  
  &__item {
    flex: 0 0 auto;
    width: 100%;
    padding: 20px;
    
    display: flex;
    flex-flow: row wrap;
    justify-content: flex-start;
    align-items: stretch;
    align-content: flex-start;
    
    & > * {
      flex: 0 0 auto;
    }
  }
  
  &--split-50 &__item {
    width: 50%;
    @media (max-width: 640px) {
      width: 100%;
    }
  }
  &--split-33 &__item {
    width: 33.3333%;
    @media (max-width: 640px) {
      width: 100%;
    }
  }
  &--gut-20 {
    margin: -10px;
  }
  &--gut-20 &__item {
    padding: 10px
  }
}
.box {
  position: relative;
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
  border-radius: 5px;
  padding: 20px;
  background: rgba(255,255,255,0.1);
  box-shadow: 0 1px 3px 0 rgba(0,0,0,.1);
}
.paragraph {
  
}
.code {
  display: block;
  margin: .5em 0;
  padding: 10px;
  border-radius: 5px;
  background: rgba(0,0,0,0.2);
  box-shadow: inset 0 1px 3px 0 rgba(0,0,0,.1);
  font-size: .9em;
}
.pre {
  white-space: pre-wrap;
  font-size: 1em;
}
.iphone {
  $iphone_bg: #333;
  
  position: relative;
  margin: .25em auto;
  
  width: 80px;
  height: 140px;
  border: 5px solid $iphone_bg;
  border-radius: 10px;
  background: #fff;
  color: $iphone_bg;
  line-height: 130px;
  font-size: 60px;
  font-weight: normal;
  text-align: center;
  overflow: hidden;
  
  animation: iphone 3s linear 0s infinite normal;
  
  &__txt {
    display: block;
    position: relative;
    z-index: 3;
  }
  
  &::before, &::after {
    content: '';
    z-index: 1;
  }
  
  &::before {
    position: absolute;
    top: 0;
    left: 50%;
    width: 60%;
    padding-top: 10%;
    border-bottom-right-radius: 5px;
    border-bottom-left-radius: 5px;
    background: $iphone_bg;
    transform: translateX(-50%);
    z-index: 2;
  }
  &::after {
    content: '';
    position: absolute;
    top: 0%;
    bottom: 0%;
    left: 0;
    width: 100%;
    background-color: $col_a;
    animation: content 3s linear 0s infinite normal;
    z-index: 1;
  }
}
@keyframes content_OLD {
  0%, 20%, 45%, 55%, 90%, 100% { top: 0%; bottom: 0%; }
  21%, 35%, 65%, 89% { top: 10%; bottom: 10%; }
}
@keyframes iphone_OLD {
  0%, 10%, 90%, 100% { transform: rotate(0deg); }
  20%, 80% { transform: rotate(-90deg); }
}
@keyframes iphone_text_OLD {
  0%, 20%, 90%, 100% { transform: rotate(0deg); }
  25%, 85% { transform: rotate(90deg); }
}
@keyframes content {
  0%, 20%, 45%, 55%, 80%, 100% { top: 0%; bottom: 0%; }
  21%, 35%, 65%, 79% { top: 10%; bottom: 10%; }
}
@keyframes iphone {
  0%, 10%, 90%, 100% { transform: rotate(0deg); }
  20%, 80% { transform: rotate(-90deg); }
}
.footer {
  
}
.color {
  &--opacity-0-5 {
    opacity: 0.5;
  }
}

```
example2
```
<html>
<head>
  <meta charset="UTF-8">
  <meta name="description" content="Free Web tutorials">
  <meta name="keywords" content="HTML,CSS,XML,JavaScript">
  <meta name="author" content="John Doe">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<p>All meta information goes in the head section...</p>

</body>
</html>

```
---

# meter tag
The meter tag defines a scalar measurement within a known range, or a fractional value. This is also known as a gauge.

Examples: Disk usage, the relevance of a query result, etc.

example1
```
<html>
<body>

<h1>The meter element</h1>

<p>The meter element is used to display a gauge:</p>

<label for="disk_c">Disk usage C:</label>
<meter id="disk_c" value="2" min="0" max="10">2 out of 10</meter><br>

<label for="disk_d">Disk usage D:</label>
<meter id="disk_d" value="0.6">60%</meter>

<p><strong>Note:</strong> The meter tag is not supported in Edge 12 (or earlier).</p>

</body>
</html>

```
HTML
example2
```
<h1>OSX-style Disk Usage <xmp>..using html5 <meter></xmp></h1>

<p>
  Macintosh HD <span class="free-space">64.54 GB free out of 120.47 GB</span></p>

<meter value="55.93" min="0" max="120.47" title="GB">
  <div class="meter-gauge">
    <span style="width: 46.42%;">Disk Usage - 55.93GB out of 120GB</span>
  </div>
</meter>  
  
<ul class="swatch">
  <li class="swatch__elem">Audio <span class="used-space">670.5 MB</span></li>
  <li class="swatch__elem">Movies <span class="used-space">10.1 GB</span></li>
  <li class="swatch__elem">Photos <span class="used-space">25.19 GB</span></li>
  <li class="swatch__elem">Apps <span class="used-space">19.31 GB</span></li>
  <li class="swatch__elem">Other <span class="used-space">660.5 MB</span></li>
</ul>

```
CSS example2

```
@import url(https://fonts.googleapis.com/css?family=Roboto);

body {
  
  font-family: "Roboto", "Lucida Grande", "Lucida", sans-serif;
  margin: 5em auto;
  background: radial-gradient(#f9f9f9 20%, #ddd 80%);
  width: 550px;
}

h1 {
  
  font-size: 1.5em;
  margin: 0 auto 2.5em;
  font-weight: 700;
}

xmp {
  
  font-family: Consolas, Monaco, monospace;
  font-size: 85%;
  color: #666;
  font-weight: 400;
}

meter {
  
  display: block;
  margin: 0 auto;
  
  width: 550px;
  height: 25px;
  
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;

  border: 1px solid #ccc;
  border-radius: 3px;
  
  /* Firefox */
  background: none; /* Required to get rid of the default background prop. */
  background-color: whiteSmoke;  
  box-shadow: 0 5px 5px -5px #333 inset;
}

meter::-webkit-meter-bar {
  
  background: none; /* Important to get rid of default background. */
  background-color: whiteSmoke;
  
  box-shadow: 0 5px 5px -5px #333 inset;
}

meter::-webkit-meter-optimum-value {
  
  transition: width .5s;
  box-shadow: 0 5px 5px -5px #999 inset;
  
  background-image: linear-gradient( 90deg, 
                                     #8bcf69 5%, 
                                     #e6d450 5%,
                                     #e6d450 15%,
                                     #f28f68 15%,
                                     #f28f68 55%,
                                     #cf82bf 55%,
                                     #cf82bf 95%,
                                     #719fd1 95%,
                                     #719fd1 100%);
  
  background-size: 100% 100%;
}

meter::-webkit-meter-optimum-value:hover {
  
  background-image: linear-gradient( 90deg, 
                                     #8bcf69 20%, 
                                     #e6d450 20%,
                                     #e6d450 40%,
                                     #f28f68 40%,
                                     #f28f68 60%,
                                     #cf82bf 60%,
                                     #cf82bf 80%,
                                     #719fd1 80%,
                                     #719fd1 100%);
  
  transition: width .5s;
  width: 100% !important; /* !important keyword used to override the inline style in ebkit browsers. */
}

meter::-moz-meter-bar {
  
  box-shadow: 0 5px 5px -5px #999 inset;
  
  background-image: linear-gradient( 90deg, 
                                     #8bcf69 5%, 
                                     #e6d450 5%,
                                     #e6d450 15%,
                                     #f28f68 15%,
                                     #f28f68 55%,
                                     #cf82bf 55%,
                                     #cf82bf 95%,
                                     #719fd1 95%,
                                     #719fd1 100%);
  
  background-size: 100% 100%;
}

p {
 
  margin: 0 auto ;
  width: 550px;
  line-height: 2.5;
}

.free-space {
  
  float: right;
}

.swatch {
  
  margin: 0; padding:0;
  margin: 5em auto;
  list-style-type: none;
  width: 550px;
  display: block;
  position: relative;
}

.swatch::before {
  
  content: '';
  width: 100%;
  height: 10px;
  outline: 0px solid #000;
  position: absolute;
  top: -20px;
  left: 0;
  border-radius: 2px;
  
  background-image: linear-gradient( 90deg, 
                                     #8bcf69 20%, 
                                     #e6d450 20%,
                                     #e6d450 40%,
                                     #f28f68 40%,
                                     #f28f68 60%,
                                     #cf82bf 60%,
                                     #cf82bf 80%,
                                     #719fd1 80%,
                                     #719fd1 100%);

}

.swatch__elem {
  
  outline: 0px solid #c00;
  float: left;
  width: 110px;
  padding-left: 5px;

  -webkit-box-sizing: border-box;
     -moz-box-sizing: border-box;
          box-sizing: border-box;
}

.used-space {
  
  display: block;
  line-height: 2;
  font-size: 85%;
  color: #666;
}

.meter-gauge {

    border: 1px solid #ccc;
    border-radius: 3px;

    background-color: whiteSmoke;
    box-shadow: 0 5px 5px -5px #333 inset;

    width: 550px;
    height: 25px;
    
    display: block;
}
  
.meter-gauge > span {
 
  height: inherit;  
  box-shadow: 0 5px 5px -5px #999 inset;
  
  background-color: blue;
  background-image: linear-gradient( 90deg, 
                                     #8bcf69 5%, 
                                     #e6d450 5%,
                                     #e6d450 15%,
                                     #f28f68 15%,
                                     #f28f68 55%,
                                     #cf82bf 55%,
                                     #cf82bf 95%,
                                     #719fd1 95%,
                                     #719fd1 100%);
  
  background-size: 100% 100%;

  display: block;
  text-indent: -9999px;
}

```
---

# nav tag
The nav tag defines a set of navigation links.

Notice that NOT all links of a document should be inside a nav element. The nav element is intended only for major blocks of navigation links.

Browsers, such as screen readers for disabled users, can use this element to determine whether to omit the initial rendering of this content.

HTML example1
```
<nav>
  <ul>
    <li><a href="index.html">Home</a></li>
    <li><a href="news.html">News</a></li>
    <li><a href="contact.html">Contact</a></li>
    <li><a href="about.html">About</a></li>
  </ul>
</nav>
<div class="main"> <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla maximus turpis quis <span id="highlight">velit accumsan</span> faucibus. Nulla eleifend erat non sapien posuere rutrum. Sed non turpis nec nibh tristique lacinia eu at nulla. Sed lacinia sagittis nisi vitae auctor. Sed non pretium neque. </p>
</div>


```
CSS example1
```
nav {
  font-size: 24px;
  font-family: sans-serif;
}

nav ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

nav li {
  display: inline;
}


nav a:link {
  color: #FF0000;
}

nav a:visited {
  color: #00FF00;
}

nav a:hover {
  color: #FF00FF;
}

nav a:active {
  color: #0000FF;
}

.main {
  text-align:center;
  background-color: #cccccc;
}

#highlight {
  background-color: #fff000;
}
```
HTML example2
```
<nav class="site-nav">
 <li class="nav-icon">
  <a>☰</a>
 </li>
 <div class="menu-top-menu-container">
  <ul id="menu-top-menu" class="menu">

   <li class="menu-item menu-item-type-custom menu-item-object-custom current-menu-item current_page_item menu-item-home">
    <a href="#">Home</a>
   </li>

   <li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-has-children">
    <a href="www.google.com">About Us</a>
    <ul class="sub-menu">
	     <li class="menu-item menu-item-type-post_type menu-item-object-page">
      <a href="#">Press and Media</a>
     </li>
	     <li class="menu-item menu-item-type-post_type menu-item-object-page">
      <a href="#">Testimonials</a>
     </li>
     	<li class="menu-item menu-item-type-post_type menu-item-object-page">
      <a href="#">Terms &#038; Conditions</a>
     </li>
	     <li class="menu-item menu-item-type-post_type menu-item-object-page">
      <a href="#">Contact Us</a>
     </li>
    </ul>
   </li>

   <li class="menu-item menu-item-type-custom menu-item-object-custom current-menu-item current_page_item menu-item-home">
    <a href="#">Home</a>
   </li>

   <li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-has-children">
    <a href="#">Menu 2</a>
    <ul class="sub-menu">
	     <li class="menu-item menu-item-type-post_type menu-item-object-page">
      <a href="#">Press and Media 2</a>
     </li>
	     <li class="menu-item menu-item-type-post_type menu-item-object-page">
      <a href="#">Testimonials 2</a>
     </li>
     	<li class="menu-item menu-item-type-post_type menu-item-object-page">
      <a href="#">Terms &#038; Conditions 2</a>
     </li>
	     <li class="menu-item menu-item-type-post_type menu-item-object-page">
      <a href="#">Contact Us 2</a>
     </li>
    </ul>
   </li>
 
  </ul>
 </div>
</nav>

<span style="color:#ffcc00">
<p>CSS and jQuery scripts of this pen are meant for making your WordPress navigation menus responsive and interactive for phones, tablets, and desktops.</p>
<p>Make sure you surround your WordPress theme's menu with the nav tag and the nav-icon code in header.php.</p>
</span>

```
CSS example2
```
*{margin:0;padding:0;} body{background:#111;}
a{color:#777;text-decoration:none;}
.site-nav, .site-nav li > ul{ background:#222; min-height:50px; }
.site-nav a { padding:0 15px; display:block; }
.site-nav ul{ list-style: none; }
.site-nav ul > li { line-height: 50px; text-align: center; }
@media screen and (min-width: 650px)
{
 .site-nav .nav-icon{ display:none; }
 .menu-top-menu-container{ display:block; }
 .site-nav li{ display: inline-block; }
 .site-nav li ul { position: absolute; display: none; }
 .site-nav li:hover ul, .site-nav li ul li { display: block; z-index:999; }
}
@media screen and ( max-width: 650px )
{
 .site-nav .nav-icon{ position:absolute; right:0px; list-style:none;}
 .site-nav .nav-icon a:hover{ cursor:pointer; }
 .site-nav .nav-icon a{ display:block; line-height:50px; color:#fc0; font-size:1.5em;}
 .site-nav > .menu-top-menu-container{ display:none; }
 .site-nav ul > li, .site-nav ul li ul li{ display:block; }
 .site-nav li > ul{ display:none; width: 100%; position:relative; }
}
.nav-fixed {position:fixed;top:0;width:100%;}
header{min-height:50px;}
p{width:350px;padding:10px;margin:0 auto;}
```

# noscript tag
The noscript tag defines an alternate content to be displayed to users that have disabled scripts in their browser or have a browser that doesn't support script.

The noscript element can be used in both head and body. When used inside head, the noscript element could only contain link,style, and meta elements.

example1
```
<body>
	<h2>This is a demo of the tag «noscript» in HTML.</h2>
	<p>Enable and disable Javascript in your web browser to see the hidden message. <br>You can use the inspector tools or an add-on like NoScript, and target cdpn.io domain to see the pen in action.</p>
  
  <noscript>
    <section class="unsupported">
      <div class="unsupported-wrapper">
				
        <h1 class="unsupported-title">
          Please enable<br>
          Javascript.
        </h1>

         <p class="unsupported-paragraph">
            This website requires Javascript in order<br>
            to work properly.
         </p>
				
      </div>
    </section>
  </noscript>
	
</body>

```
example2
```
<script>
document.write("Merhaba Dünya!")
</script>
<noscript>Tarayıcınız javascript desteklemiyor!</noscript>

```
---
# object tag
The object tag defines a container for an external resource.

The external resource can be a web page, a picture, a media player, or a plug-in application.

example
```
<html>
<body>

<h1>The object element</h1>

<object data="snippet.html" width="500" height="200">
</object>
 
</body>
</html>

```
---
# ol tag
The ol tag defines an ordered list. An ordered list can be numerical or alphabetical.

The li tag is used to define each list item.

example1
```
<html>
<body>

<h1>Specify list type with CSS</h1>

<ol style="list-style-type:upper-roman">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol style="list-style-type:lower-alpha">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

</body>
</html>

```
example2
```
<html>
<head>
<style>
ol.a {list-style-type: armenian;}
ol.b {list-style-type: cjk-ideographic;}
ol.c {list-style-type: decimal;}
ol.d {list-style-type: decimal-leading-zero;}
ol.e {list-style-type: georgian;}
ol.f {list-style-type: hebrew;}
ol.g {list-style-type: hiragana;}
ol.h {list-style-type: hiragana-iroha;}
ol.i {list-style-type: katakana;}
ol.j {list-style-type: katakana-iroha;}
ol.k {list-style-type: lower-alpha;}
ol.l {list-style-type: lower-greek;}
ol.m {list-style-type: lower-latin;}
ol.n {list-style-type: lower-roman;}
ol.o {list-style-type: upper-alpha;}
ol.p {list-style-type: upper-latin;}
ol.q {list-style-type: upper-roman;}
ol.r {list-style-type: none;}
ol.s {list-style-type: inherit;}
</style>
</head>
<body>

<h1>All the different list types for ol with CSS</h1>

<ol class="a">
  <li>Armenian type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="b">
  <li>Cjk-ideographic type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="c">
  <li>Decimal type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="d">
  <li>Decimal-leading-zero type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="e">
  <li>Georgian type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="f">
  <li>Hebrew type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="g">
  <li>Hiragana type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="h">
  <li>Hiragana-iroha type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="i">
  <li>Katakana type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="j">
  <li>Katakana-iroha type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="k">
  <li>Lower-alpha type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="l">
  <li>Lower-greek type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="m">
  <li>Lower-latin type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="n">
  <li>Lower-roman type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="o">
  <li>Upper-alpha type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="p">
  <li>Upper-latin type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="q">
  <li>Upper-roman type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="r">
  <li>None type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="s">
  <li>inherit type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

</body>
</html>

```
---

# optgrouop tag
the optgroup tag is used to group related options in a select element (drop-down list).

If you have a long list of options, groups of related options are easier to handle for a user.

example1

```
<html>
<body>

<h1>The optgroup element</h1>

<p>The optgroup tag is used to group related options in a drop-down list:</p>

<form action="/action_page.php">
  <label for="cars">Choose a car:</label>
  <select name="cars" id="cars">
    <optgroup label="Swedish Cars">
      <option value="volvo">Volvo</option>
      <option value="saab">Saab</option>
    </optgroup>
    <optgroup label="German Cars">
      <option value="mercedes">Mercedes</option>
      <option value="audi">Audi</option>
    </optgroup>
  </select>
  <br><br>
  <input type="submit" value="Submit">
</form>
 
</body>
</html>

```
example2
```
<p>Select your game:
	<select name="games">
		<optgroup label="PS4">
			<option>PS4 Game 1</option>
			<option>PS4 Game 2</option>
			<option>PS4 Game 3</option>
		</optgroup>
		<optgroup label="PS3">
			<option>PS3 Game 1</option>
			<option>PS3 Game 2</option>
			<option>PS3 Game 3</option>
		</optgroup>
		<optgroup label="XBOX 360">
			<option>XBOX 360 Game 1</option>
			<option>XBOX 360 Game 2</option>
		</optgroup>
		<optgroup label="XBOX ONE">
			<option>XBOX ONE Game 1</option>
			<option>XBOX ONE Game 2</option>
			<option>XBOX ONE Game 3</option>
			<option>XBOX ONE Game 4</option>
			<option>XBOX ONE Game 5</option>
		</optgroup>
	</select>
</p>
<br><a href="http://www.cssinhtml.com" target="_blank">Go to CSS in HTML</a>

```
---
# option tag
The option tag defines an option in a select list.

option elements go inside a select, optgroup, or datalist element.

HTML example1
```
<h1>Search in select "option" tag</h1>
<select multiple name="selectMenu" id="selectMenu" style="width:100px" size=10>
<option value ="item 1">item 1</option>
<option value ="item 2">item 2</option>
<option value ="thing 3">thing 3</option>
<option value ="item 4">item 4</option>
<option value ="stuff 5">stuff 5</option>
<option value ="stuff 6">stuff 6</option>
<option value ="stuff 7">stuff 7</option>
<option value ="item 8">item 8</option>
</select>

<p>Search within this list</p>
<input type=text name="search" id="search" onkeypress="searchItems();">
<br>
<input type=button value="Search" onclick="searchItems();">
<input type=button value="Reset List" onclick="resetList();">
  
  <div class="Ref">
    check out our website
    <a href="http://aliensolutions.net/">Alien solutions</a> | <a href="http://aliensolutions.net/themes/?theme=Flat-UI">Download Flat UI framework here</a>
  </div>

```
CSS example1
```
@import url(https://fonts.googleapis.com/css?family=Oxygen:400,300);
h1{
  with:100%;
  background:#34495E;
  color:#fff;
  padding:10px 20px;
  font-family: 'Oxygen', sans-serif;
  font-weight:300;
}
.Ref{
  border-top:3px solid #2980B9;
  margin:10px 0px 50px 0px;
  font-family: 'Oxygen', sans-serif;
  
}

```
example2
```
<html>
<body>

<h1>The option element</h1>

<label for="cars">Choose a car:</label>

<select id="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="opel">Opel</option>
  <option value="audi">Audi</option>
</select>
  
</body>
</html>

```
---
# output tag
The output tag is used to represent the result of a calculation (like one performed by a script).

example


```
<html>
<body>

<h1>The output element</h1>

<form oninput="x.value=parseInt(a.value)+parseInt(b.value)">
<input type="range" id="a" value="50">
+<input type="number" id="b" value="25">
=<output name="x" for="a b"></output>
</form>

<p><strong>Note:</strong> The output element is not supported in Edge 12 (or earlier).</p>

</body>
</html>

```
---
# paragraph tag
The p tag defines a paragraph.

Browsers automatically add a single blank line before and after each <p> element.

example
```
<html>
<head>
<style>
p {
  color: navy;
  text-indent: 30px;
  text-transform: uppercase;
}
</style>
</head>
<body>

<h1>Style paragraphs with CSS</h1>

<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>

<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>

</body>
</html>

```
---
# param tag

The param tag is used to define parameters for an object element.

example
```
<p><b>Not:</b> internet explorer 8 ve önceki sürümlerinde .waw uzantısını desteklemez.</p>

<object data="http://w3tr.com/file/flut1.mp3">
<param name="oynat" value="true">
</object>
```
---
# picture tag
The picture tag gives web developers more flexibility in specifying image resources.

The most common use of the picture element will be for art direction in responsive designs. Instead of having one image that is scaled up or down based on the viewport width, multiple images can be designed to more nicely fill the browser viewport.

The picture element contains two tags: one or more source tags and one img tag.

The browser will look for the first source element where the media query matches the current viewport width, and then it will display the proper image (specified in the srcset attribute). The img element is required as the last child of the picture element, as a fallback option if none of the source tags matches.

example1

```
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<h1>The picture element</h1>

<p>Resize the browser window to load different images.</p>

<picture>
  <source media="(min-width:650px)" srcset="img_pink_flowers.jpg">
  <source media="(min-width:465px)" srcset="img_white_flower.jpg">
  <img src="img_orange_flowers.jpg" alt="Flowers" style="width:auto;">
</picture>

</body>
</html>

```
---
# pre tag

the pre tag defines preformatted text.

Text in a pre element is displayed in a fixed-width font, and the text preserves both spaces and line breaks. The text will be displayed exactly as written in the HTML source code.

example

```
<html>
<body>

<h1>The pre element</h1>

<pre>
Text in a pre element
is displayed in a fixed-width
font, and it preserves
both      spaces and
line breaks
</pre>

</body>
</html>

```
---
# progress tag 
The progress tag represents the completion progress of a task.

Tip: Always add the label tag for best accessibility practices!

example1 html 
```
<ul>
	<li>
		<h2>Frontend</h2>
		
		<!-- HTML5 -->
    <p style="width:80%" data-value="80">HTML5</p>
		<progress max="100" value="80" class="html5">
			
			<div class="progress-bar">
				<span style="width: 80%">80%</span>
			</div>
		</progress>
		
		<!-- CSS3 -->
    <p style="width:60%" data-value="60">CSS3</p>
		<progress max="100" value="60" class="css3">
			
			<div class="progress-bar">
				<span style="width: 60%">60%</span>
			</div>
		</progress>
		
		<!-- jQuery -->
    <p style="width:50%" data-value="50">jQuery</p>
		<progress max="100" value="50" class="jquery">
			
			<div class="progress-bar">
				<span style="width: 50%">50%</span>
			</div>
		</progress>
		
	</li>
	<li>
		<h2>Backend</h2>
		
    <!-- Python -->
    <p style="width:75%" data-value="75">Python</p>
		<progress max="100" value="75" class="python">
			
			<div class="progress-bar">
				<span style="width: 75%">75%</span>
			</div>
		</progress>
		
		<!-- PHP -->
    <p style="width:65%" data-value="65">PHP</p>
		<progress max="100" value="65" class="php">
			
			<div class="progress-bar">
				<span style="width: 65%">65%</span>
			</div>
		</progress>
		
		<!-- Node.js -->
    <p style="width:35%" data-value="35">Node.js</p>
    <progress max="100" value="35" class="node-js">
			
			<div class="progress-bar">
				<span style="width: 35%">35%</span>
			</div>
		</progress>		
		
	</li>
</ul>

<p>Article - <a href="https://css-tricks.com/html5-progress-element/">https://css-tricks.com/html5-progress-element/</a></p>

```
CSS example1
```
@import url(https://fonts.googleapis.com/css?family=Expletus+Sans);



* { 
	margin:0; padding:0; 
	box-sizing: border-box;
}

body {
margin: 50px auto 0;
max-width: 800px;

font-family: "Expletus Sans", sans-serif;
}

li {
  width: 50%;
	float: left;
	list-style-type: none;
	
	padding-right: 5.3333333%;
}

li:nth-child(even) { margin-bottom: 5em;}

h2 {
	margin: 0 0 1.5em;
	border-bottom: 1px solid #ccc;
	padding: 0 0 .25em;
}
progress:not(value) {

}
progress[value] {
	
	appearance: none;
	
	border: none;
	
	
	width: 100%; height: 20px;
	  background-color: whiteSmoke;
	  border-radius: 3px;
	  box-shadow: 0 2px 3px rgba(0,0,0,.5) inset;
	
	color: royalblue;
	position: relative;
	margin: 0 0 1.5em; 
}



progress[value]::-webkit-progress-bar {
	background-color: whiteSmoke;
	border-radius: 3px;
	box-shadow: 0 2px 3px rgba(0,0,0,.5) inset;
}

progress[value]::-webkit-progress-value {
	position: relative;
	
	background-size: 35px 20px, 100% 100%, 100% 100%;
	border-radius:3px;
	
	
	animation: animate-stripes 5s linear infinite;
}

@keyframes animate-stripes { 100% { background-position: -100px 0; } }


progress[value]::-webkit-progress-value:after {

	content: '';
	position: absolute;
	
	width:5px; height:5px;
	top:7px; right:7px;
	
	background-color: white;
	border-radius: 100%;
}


progress[value]::-moz-progress-bar {
	
	background-image:
	-moz-linear-gradient( 135deg,
													 transparent,
													 transparent 33%,
													 rgba(0,0,0,.1) 33%,
													 rgba(0,0,0,.1) 66%,
													 transparent 66%),
    -moz-linear-gradient( top,
														rgba(255, 255, 255, .25),
														rgba(0,0,0,.2)),
     -moz-linear-gradient( left, #09c, #f44);
	
	background-size: 35px 20px, 100% 100%, 100% 100%;
	border-radius:3px;
	
	/* Firefox doesn't support CSS3 keyframe animations on progress element. Hence, we did not include animate-stripes in this code block */
}

/* Fallback technique styles */
.progress-bar {
	background-color: whiteSmoke;
	border-radius: 3px;
	box-shadow: 0 2px 3px rgba(0,0,0,.5) inset;

	
	width: 100%; height:20px;
}

.progress-bar span {
	background-color: royalblue;
	border-radius: 3px;
	
	display: block;
	text-indent: -9999px;
}

p[data-value] { 
  
  position: relative; 
}



p[data-value]:after {
	content: attr(data-value) '%';
	position: absolute; right:0;
}





.html5::-webkit-progress-value,
.python::-webkit-progress-value  {
	/* Gradient background with Stripes */
	background-image:
	-webkit-linear-gradient( 135deg,
													 transparent,
													 transparent 33%,
													 rgba(0,0,0,.1) 33%,
													 rgba(0,0,0,.1) 66%,
													 transparent 66%),
    -webkit-linear-gradient( top,
														rgba(255, 255, 255, .25),
														rgba(0,0,0,.2)),
     -webkit-linear-gradient( left, #09c, #f44);
}

.css3::-webkit-progress-value,
.php::-webkit-progress-value 
{
	
	background-image:
	-webkit-linear-gradient( 135deg,
													 transparent,
													 transparent 33%,
													 rgba(0,0,0,.1) 33%,
													 rgba(0,0,0,.1) 66%,
													 transparent 66%),
    -webkit-linear-gradient( top,
														rgba(255, 255, 255, .25),
														rgba(0,0,0,.2)),
     -webkit-linear-gradient( left, #09c, #ff0);
}

.jquery::-webkit-progress-value,
.node-js::-webkit-progress-value 
{
	/* Gradient background with Stripes */
	background-image:
	-webkit-linear-gradient( 135deg,
													 transparent,
													 transparent 33%,
													 rgba(0,0,0,.1) 33%,
													 rgba(0,0,0,.1) 66%,
													 transparent 66%),
    -webkit-linear-gradient( top,
														rgba(255, 255, 255, .25),
														rgba(0,0,0,.2)),
     -webkit-linear-gradient( left, #09c, #690);
}



.html5::-moz-progress-bar,
.php::-moz-progress-bar {
	
	background-image:
	-moz-linear-gradient( 135deg,
													 transparent,
													 transparent 33%,
													 rgba(0,0,0,.1) 33%,
													 rgba(0,0,0,.1) 66%,
													 transparent 66%),
    -moz-linear-gradient( top,
														rgba(255, 255, 255, .25),
														rgba(0,0,0,.2)),
     -moz-linear-gradient( left, #09c, #f44);
}

.css3::-moz-progress-bar,
.php::-moz-progress-bar {
{
	
	background-image:
	-moz-linear-gradient( 135deg,
													 transparent,
													 transparent 33%,
													 rgba(0,0,0,.1) 33%,
													 rgba(0,0,0,.1) 66%,
													 transparent 66%),
    -moz-linear-gradient( top,
														rgba(255, 255, 255, .25),
														rgba(0,0,0,.2)),
     -moz-linear-gradient( left, #09c, #ff0);
}

.jquery::-moz-progress-bar,
.node-js::-moz-progress-bar {
	/* Gradient background with Stripes */
	background-image:
	-moz-linear-gradient( 135deg,
													 transparent,
													 transparent 33%,
													 rgba(0,0,0,.1) 33%,
													 rgba(0,0,0,.1) 66%,
													 transparent 66%),
    -moz-linear-gradient( top,
														rgba(255, 255, 255, .25),
														rgba(0,0,0,.2)),
     -moz-linear-gradient( left, #09c, #690);
}


  

```
---
example2 HTML
```
<div class="playground">
  <div class="bar-container">
    <h2>HTML</h2>
    <ul>
      <li>
       <span class="css-progressbar bar"/>
      </li>
    </ul>
  </div>
  <div class="bar-container">
    <h2>HTML5</h2>
    <progress class="progressTag" value="0" max="100"/>
  </div>
  <div class="bar-container">
    <h2>SVG</h2>
    <svg class="progressSvg" height="150" width="150">
      <g class="progress-container">
        <line 
            x1="0"
            y1="50%"
            x2="100%"
            y2="50%"
            stroke-width="20" />
      </g>
      <g class="progress-content">
        <line
            x1="0"
            y1="50%"
            x2="100%"
            y2="50%"
            fill="transparent"
            stroke-width="20" />
      </g>
    </svg>
  </div>
  
</div>

```

CSS example2
```
body {
  position: absolute;
  padding: 0;
  margin: 0;
  width: 100%;
  height: 100%;
  background-color: #41b882;
  display: flex;
  align-items: center;
  justify-content: center;
  .playground {
    background-color: #fff;
    border-radius: 6px;
    box-shadow: 0 1px 3px 0 rgba(0,0,0,.12), 0 2px 1px 0 rgba(0,0,0,.12);
    width: 600px;
    height: 200px;
    display: flex;
    padding: 1rem;
    .bar-container {
      h2 {
        position: absolute;
        text-align: center;
        top: 10px;
        width: 100%;
      }
      position: relative;
      height: 100%;
      flex: 0 0 30%;
      margin: 0 auto;
      background-color: #41b882;
      display: flex;
      align-items: center;
      justify-content: center;
      // **** CSS progress bar ****
      ul {
        position: relative;
        padding: 0;
        list-style: none;
        width: 150px;
        li {
          background-color: #fff;
          height:20px; 
          border-radius:10px;
          .bar {
            position: absolute;
            border-radius: 10px; 
            background-color: #35495e;
            height: 20px;
            &:after  {
              -webkit-box-sizing: border-box;
              box-sizing: border-box;
              content: "";
              width: 27px;
              height: 27px;
              position: absolute;
              top: -3px;
              right: 0;
              border-radius: 50%;
              background-color: #607d8b;
            }
          }
          .css-progressbar {
            width: 80%; 
            -moz-animation: css-progressbar 2s ease-out;
            -webkit-animation: css-progressbar 2s ease-out;
          }
        }
      }
      // **** HTML TAG progress bar ****
      .progressTag {
        -webkit-appearance: none;
        -moz-appearance: none;
        appearance: none;
        display: block;
        width: 150px;
        height: 20px;
        border-radius: 7px;
        color: #35495e;
      }
      progress::-webkit-progress-bar {
        background-color: #eee;
        border-radius: 8px;
      }
      progress::-webkit-progress-value {
        background-color: #35495e;
        border-radius: 8px;
      }
      progress::-moz-progress-bar {
        background-color: #eee;
        border-radius: 8px;
      }
      // **** SVG progress bar ****
      .progressSvg {
        border-radius: 7px;
        color: #35495e;
        .progress-container {
          stroke: #eee;
        }
        .progress-content {
          stroke: #35495e;
        }
        
        .progress-content > line {
          stroke-dasharray: 100%;
          stroke-dashoffset: 20%;
          -moz-animation: svg-progress 2s ease-out;
          -webkit-animation: svg-progress 2s ease-out;
        }
      }
    }
  }
}

 @-webkit-keyframes svg-progress {
   0% {
     stroke-dashoffset: 100%;
   }
   100% {
     stroke-dashoffset: 20%;
   }
}

@-moz-keyframes svg-progress {
   0% {
     stroke-dashoffset: 100%;
   }
   100% {
     stroke-dashoffset: 20%;
   }
}

@-webkit-keyframes css-progressbar { 
  0%  { 
    width: 0px;
  } 
  100% { 
    width: 80%;
  }  
}

@-moz-keyframes css-progressbar {
  0% { 
    width: 0px;
  } 
  100% { 
    width: 80%;
  }  
}

```
---

# q tag
The q tag defines a short quotation.

Browsers normally insert quotation marks around the quotation.

example
```
<html>
<body>

<h1>The q element</h1>

<p>WWF's goal is to: 
<q>Build a future where people live in harmony with nature.</q>
We hope they succeed.</p>

</body>
</html>

```
---
# parentheses tag
The rp tag can be used to provide parentheses around a ruby text, to be shown by browsers that do not support ruby annotations.

Use rp together with ruby and rt: The ruby element consists of one or more characters that needs an explanation/pronunciation, and an rt element that gives that information, and an optional rp element that defines what to show for browsers that not support ruby annotations.

example1
```
<h3>Example in English text to demonstrate
how ruby annotations are displayed by the browser.</h3>
	<p>
	From oranges we can create
	<ruby> OJ <rp>(</rp><rt>Orange Juice</rt><rp>)</rp></ruby>
	</p>
	
	<h3>Example in logographic language.</h3>
	<ruby>
	東京
		<rp> (</rp>
		<rt>Tō kyō</rt>
		<rp>)</rp>
	</ruby>
<br>
<br><a href="http://www.cssinhtml.com" target="_blank">Go to CSS in HTML</a>

```
example2
```
<html>
<body>

<h1>The rp element</h1>

<ruby>
漢 <rp>(</rp><rt>ㄏㄢˋ</rt><rp>)</rp>
</ruby>

</body>
</html>

```
---

# rt tag

The rt tag defines an explanation or pronunciation of characters (for East Asian typography) in a ruby annotation.

Use rt together with ruby and rp: The ruby element consists of one or more characters that needs an explanation/pronunciation, and an rt element that gives that information, and an optional rp element that defines what to show for browsers that not support ruby annotations.

example
```
<ruby>
漢 <rt> ㄏㄢˋ </rt>
</ruby>

```
# ruby tag

he ruby tag specifies a ruby annotation.

A ruby annotation is a small extra text, attached to the main text to indicate the pronunciation or meaning of the corresponding characters. This kind of annotation is often used in Japanese publications.

Use ruby together with rt and rp: The ruby element consists of one or more characters that needs an explanation/pronunciation, and an rt element that gives that information, and an optional rp element that defines what to show for browsers that do not support ruby annotations.

example
```
<html>
<body>

<h1>The ruby and rt elements</h1>

<ruby>
 漢 <rt> ㄏㄢˋ </rt>
</ruby>

</body>
</html>

```
---
# s tag
The s tag specifies text that is no longer correct, accurate or relevant. The text will be displayed with a line through it.

The s tag should not be used to define deleted text in a document, use the del tag for that.

example1

html
```
<article class="news-item">
    <h1>WordPress 4.4 Updates</h1>
    <section class="summary" aria-label="Summary">
    WordPress 4.4 (code-named <s cite="https://codex.wordpress.org/Version_4.4">Bobby Brown</s> Clifford Brown) was released to the public on the 8th of December 2015.
    </section>
    <section class="main-content" aria-label="Main Content">
    <p>There were several changes in V4.4 including the following</p>
    <ul>
        <li>New default theme - <s>Twenty Fifteen</s> Twenty Sixteen</li>
        <li>Responsive image support (image elements in the content now support display based rendering)
        <li>Additional embed object support such as Cloudup, Reddit Comments etc</li>
    <ul>
    </section>
</article>

```
CSS 

example1
```
body {
  color: #333;
  font-family: Tahoma, sans-serif;
  font-size: 16px;
  line-height: 1.25;
}

h1 {
  color: #1C94C6;
  font-family: Georgia, serif;
  font-size: 26px;
  font-weight: normal;
}

```
# samp tag
The samp tag is used to define sample output from a computer program. The content inside is displayed in the browser's default monospace font.

example

```
<html>
<body>

<h1>The samp element</h1>

<p>Message from my computer:</p>

<p><samp>File not found.<br>Press F1 to continue</samp></p>

</body>
</html>

```
---
# script tag
The script tag is used to embed a client-side script (JavaScript).

The script element either contains scripting statements, or it points to an external script file through the src attribute.

Common uses for JavaScript are image manipulation, form validation, and dynamic changes of content.

example1
```
<html>
<body>

<h1>The script element</h1>

<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script> 

</body>
</html>

```
---
# section tag

The section tag defines a section in a document.

example1 html
```
<link href='https://fonts.googleapis.com/css?family=Lobster+Two' rel='stylesheet' type='text/css'>
<body>
<section class="canvas">
<h1 >My Summer Vacation</h1>
  
<p class="content-style ">This summer I went to Camp Smurfabunch. I was there for 2 weeks and had mega fun times. I was the fastest kayaker in the whole camp and won a first place ribbon. I learned to tie knots, dive off a pier, and lick toads.</p>
  
<p class="content-style ">I met new friends Ketchel, Caleb, and Sarah. I hope they come visit me later this summer but even if they can't &mdash; I'll see them next summer.</p>

<hr>

<p class="content-style ">Later that summer I got to go to Wisconsin Dells with my family. We stayed at The Wilderness which has both inside and outside water parks. My mom was scared to go down the four-person funnel ride, but she did anyway and ended up liking it.</p>

<p class="content-style ">We went go karting at Mt. Zues (or something, I can't remember the name but there was an old god dude holding a lightning bolt as the logo). I beat my brother and dad on the first 2 laps but dad pulled ahead and beat me on the last lap.</p>

<hr>

<p class="content-style ">The last thing I did this summer was go shopping for school clothes and supplies. I got a Trapper Keeper with KISS on it. And like fifty erasers because I make mistakes a lot lololol.</p>

<p class="content-style ">I don't want to go back to school but I know once I get used to it, it will be fine again. I'd rather just go down waterslides all day.</p>
</section>

```
example2 html
```
<h1>Accessible CSS Accordion Menus <sup><a href="#notes">#notes</a></sup></h1>
  
  <h2>Radio based accordion</h2>
  <big><em>Only one collapsible section can be open at any given time. Use the <pre>TAB</pre> key to focus on the group and then navigate through it with the <pre>UP</pre> and <pre>DOWN</pre> keys.</em></big>

  <section class="faq-container">

    <input id="faq1a" name="faq1" type="radio" checked="checked">
    <label for="faq1a">A surprise party?</label>
    <article>
      <p>Mr. Worf, I hate surprise parties.</p>
    </article>

    <input id="faq1b" name="faq1" type="radio">
    <label for="faq1b">I've had twelve years to think about it.</label>
    <article>
      <p>And if I had it to do over again, I would have grabbed the phaser and pointed it at you instead of them.</p>
    </article>

    <input id="faq1c" name="faq1" type="radio">
    <label for="faq1c">I would *never* do that to you.</label>
    <article>
      <p>I will obey your orders. I will serve this ship as First Officer. And in an attack against the Enterprise, I will die with this crew. But I will not break my oath of loyalty to Starfleet.</p>
    </article>

    <input id="faq1d" name="faq1" type="radio">
    <label for="faq1d">Could someone survive inside a transporter buffer for 75 years?</label>
    <article>
      <p>I suggest you drop it, Mr. Data. This is not about revenge.</p>
    </article>

  </section>
  
  <h2>Checkbox based accordion</h2>
  <big><em>Multiple collapsible sections can be open at any given time. Use the <pre>TAB</pre> key to focus on the group and navigate through the section labels, <pre>SHIFT+TAB</pre> can be used to navigate backwards. Pressing <pre>SPACE</pre> on an active section will toggle the article visibility.</em></big>

  <section class="faq-container">

    <input id="faq2a" name="faq2" type="checkbox" checked="checked">
    <label for="faq2a">What's a knock-out like you doing in a computer-generated gin joint like this?</label>
    <article>
      <ul>
        <li>Congratulations - you just destroyed the Enterprise.</li>
        <li>Worf, It's better than music. It's jazz.</li>
        <li>Wait a minute - you've been declared dead.</li>
        <li>A lot of things can change in twelve years, Admiral.</li>
      </ul>
    </article>

    <input id="faq2b" name="faq2" type="checkbox">
    <label for="faq2b">Mr. Worf, you do remember how to fire phasers?</label>
    <article>
      <ul>
        <li>Some days you get the bear, and some days the bear gets you.</li>
        <li>Your only concern is with how you obey my orders.</li>
        <li>Fear is the true enemy, the only enemy.</li>
        <li>For an android with no feelings, he sure managed to evoke them in others.</li>
      </ul>
    </article>

    <input id="faq2c" name="faq2" type="checkbox">
    <label for="faq2c">Yesterday I did not know how to eat gagh.</label>
    <article>
      <p>Now we know what they mean by 'advanced' tactical training.</p>
    </article>

    <input id="faq2d" name="faq2" type="checkbox">
    <label for="faq2d">Are you up for promotion?</label>
    <article>
      <p>Why don't we just give everybody a promotion and call it a night - 'Commander'?</p>
    </article>

  </section>
  
  <h2 id="notes">Notes</h2>
  <h3><em>This is my initial stab at a pure CSS accordion solution that is accessible. With inspiration from the following pens: <a href="https://codepen.io/simtoalev/pen/jAJzjg">Pure CSS Accordion Content With Animation</a>, and <a href="https://codepen.io/anzjoy/pen/bahAv">Pure Css Accordion Menu</a>. However, it's still far from perfect. So feel free to fork this and improve on it. Issues I've considered include:</em></h3>
  <ul>
    <li>Is it semantically correct?  Would swapping the SECTION tag for a definition list (DL) and wrapping the input and label elements in a DT tag and the answer in a DD tag be better?</li>
    <li>The Font Awesome icons are injected via CSS. Do screen readers see these? Must test.</li>
    <li>The question mark to the left would probably become repetative if it is seen screen reader.  What would it read out, F29C is a private use code point?</li>
    <li>The chevron to the right wraps awkwardly on narrow viewports.  It also has the same accessibility issues as the question mark, with the added issue that it is used to indicate state.</li>
    <li>My transitions on the ARTICLE tag aren't firing, haven't investigated yet.</li>
    <li>No, the colours aren't accessible. <i class="fa fa-frown-o"></i></li>
  </ul>
  <h3><em>Changes</em></h3>
  <ul>
    <li>I removed the <strong>aria-hidden</strong> attribute from the <strong>input</strong> tags as this was causing the screen reader (ChromeVox) to ignore the associated label text.</li>
  </ul>

```
example2 CSS
```
@import 'https://fonts.googleapis.com/css?family=Source+Sans+Pro:400,600,700';

body {
  background: #FFF;
  font-family: 'Source Sans Pro';
  font-weight: 400;
}

h1 {
  color: #333;
  font-size: 36px;
  font-weight: normal;
  text-align: center;
}
h1 sup a { color: #999; font-size: 14px; text-decoration: none; }
h1 sup a:hover { color: #666; text-decoration: none; }
h1 sup a:focus,
h1 sup a:active { color: #666; text-decoration: underline; }

h2 {
  color: #333;
  font-size: 30px;
  font-weight: normal;
  text-align: left;
}

big {
  color: #333;
  font-size: 20px;
  font-weight: normal;
  margin: 0;
  padding: 0;
  text-align: left;
}
big pre {
  display: inline-block;
  font-weight: bold;
  margin: 0;
  padding: 0;
}

.faq-container {
  text-align: left;
  margin: 10px auto 30px auto;
  position: relative;
}
.faq-container article p { margin: 10px 15px 15px 15px; }
.faq-container input[type=checkbox],
.faq-container input[type=radio] {
  background-color: transparent;
  border: 1px solid transparent;
  height: 1px;
  position: absolute;
  width: 1px;
  margin: 4px 0 0 0;
  outline: none;
}
.faq-container input[type=checkbox] + label,
.faq-container input[type=radio] + label {
  background: #EEEEEE;
  border-bottom: 1px solid #fff;
  color: #333;
  cursor: pointer;
  display: block;
  font-size: 18px;
  font-weight: normal;
  line-height: 32px;
  padding: 10px 15px;
  position: relative;
  z-index: 20;
}
.faq-container input[type=checkbox] + label:before,
.faq-container input[type=radio] + label:before,
.faq-container input[type=checkbox] + label:after,
.faq-container input[type=radio] + label:after {
  display: inline-block;
  font-family: FontAwesome;
  font-size: 24px;
  font-style: normal;
  font-weight: normal;
  text-decoration: inherit;
}
.faq-container input[type=checkbox] + label:before,
.faq-container input[type=radio] + label:before {
  content: "\f29c";
  padding-right: 10px;
}
.faq-container input[type=checkbox] + label:after,
.faq-container input[type=radio] + label:after {
  content: "\f054";
  float: right;
  padding-left: 10px;
}
.faq-container input[type=checkbox] + label:hover,
.faq-container input[type=radio] + label:hover { background: #D6D6D6; }
.faq-container input[type=checkbox]:checked + label,
.faq-container input[type=radio]:checked + label { background: #EEEEEE; }
.faq-container input[type=checkbox]:focus + label,
.faq-container input[type=radio]:focus + label { background: #BEBEBE; }
.faq-container input[type=checkbox]:checked + label:hover,
.faq-container input[type=radio]:checked + label:hover { background: #D6D6D6; }
.faq-container input[type=checkbox]:checked + label:after,
.faq-container input[type=radio]:checked + label:after {
	-webkit-transform: rotate(90deg);
	   -moz-transform: rotate(90deg);
	    -ms-transform: rotate(90deg);
	     -o-transform: rotate(90deg);
	        transform: rotate(90deg);
}
.faq-container input[type=checkbox] + label + article,
.faq-container input[type=radio] + label + article {
  display: none;
  /* display: none; - Content is ignored by screen readers, additionally stops tabbing through hidden content */
  height: 0;
  max-height: 0;
  overflow: hidden;
  
  -webkit-transition: all 1.5s ease-in-out;
  -moz-transition: all 1.5s ease-in-out;
  -o-transition: all 1.5s ease-in-out;
  -ms-transition: all 1.5s ease-in-out;
  transition: all 1.5s ease-in-out;
}
.faq-container input[type=checkbox]:checked + label + article,
.faq-container input[type=radio]:checked + label + article {
  display: block;
  height: auto;
  max-height: 2000px;
  -webkit-transition: all 1.5s ease-in-out;
  -moz-transition: all 1.5s ease-in-out;
  -o-transition: all 1.5s ease-in-out;
  -ms-transition: all 1.5s ease-in-out;
  transition: all 1.5s ease-in-out;
}
```
---
# select tag
The select element is used to create a drop-down list.

The select element is most often used in a form, to collect user input.

The name attribute is needed to reference the form data after the form is submitted (if you omit the name attribute, no data from the drop-down list will be submitted).

The id attribute is needed to associate the drop-down list with a label.

The option tags inside the select element define the available options in the drop-down list.

Example1 

HTML
```
<div class="container">

		<div class="selected-item">
			<p>You Selected Country : <span>Select</span></p>
		</div>

		<select name="" id="cusSelectbox">
			<option value="Select">Select</option>
			<option value="India">India</option>
			<option value="Nepal">Nepal</option>
			<option value="Bangladesh">Bangladesh</option>
			<option value="Sri Lanka">Sri Lanka</option>
		</select>
	
		<div class="feaBlock">
			<ol>
				<li>Up & Down key works on list items.</li>
				<li>Key enter works on list items.</li>
				<li>Scrollbar hide, but you can scroll the list items.</li>
			</ol>
		</div>

	</div>

```
example1 CSS 
```
@import url(https://fonts.googleapis.com/css?family=Roboto);
/* variables */
/* default style */
body {
  background-color: #fff;
  color: #333;
  font-family: "Roboto", arial, sans-serif;
  font-size: 16px;
}
/* common style */
* {
  margin: 0;
  padding: 0;
}
*,
*:after,
*:before {
  box-sizing: border-box;
}
* {
  outline: none;
}
::-webkit-scrollbar { 
  display: none; 
}
/* */
.container {
	margin: 0 auto;
	max-width: 400px;
  text-align: center;
}
.selected-item {
  margin: 20px 0;
}
/* custom select style */
.cusSelBlock {
  height: 50px;
  min-width: 250px;
}
#cusSelectbox {
  height: 100%;
  width: 100%;
}
.s-hidden {
  visibility: hidden;
}
.cusSelBlock {
  display: inline-block;
  position: relative;
  -webkit-perspective: 800px;
          perspective: 800px;
}
.selectLabel {
  position: absolute;
  left: 0;
  top: 0;
  z-index: 9999;

  background-color: #fff;
  border: 1px solid #333;
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.1);
  color: #333;
  cursor: pointer;
  display: block;

  height: 100%;
  width: 100%;

  letter-spacing: 2px;
  line-height: 50px;
  padding: 0 50px 0 20px;
  text-align: left;

  -webkit-transform-style: preserve-3d;
          transform-style: preserve-3d;
  -webkit-transform-origin: 50% 0%;
          transform-origin: 50% 0%;

  -webkit-transition: -webkit-transform 300ms;
  transition: -webkit-transform 300ms;
  transition: transform 300ms;
  transition: transform 300ms, -webkit-transform 300ms;

  -webkit-backface-visibility: hidden;
  -webkit-touch-callout: none;
  -webkit-user-select: none;
     -moz-user-select: none;
      -ms-user-select: none;
          user-select: none;
  &:after {
    content: '\25BC';
    border-left: 1px solid #333;
    color: #333;
    font-size: 12px;
    line-height: 17px;
    padding: 10px;
    text-align: center;

    position: absolute;
    right: 0px;
    top: 15%;

    height: 70%;
    width: 50px;
  }
  &:active {
    -webkit-transform: rotateX(30deg);
            transform: rotateX(30deg);
    &:after {
      content: '\25B2';
    }
  }
  &.active {
    &:after {
      content: '\25B2';
    }
    &+.options {
      //height: 200px;
      //overflow-y: scroll;
    }
  }
}
::-webkit-scrollbar { 
  display: none; 
}
.options {
  position: absolute;
  top: 50px;

  height: 1px;
  width: 100%;
  li {
    background-color: rgb(255,255,255);
    border-left: 1px solid #333;
    border-right: 1px solid #333;
    border-bottom: 1px solid #333;
    cursor: pointer;
    display: block;
    line-height: 50px;
    list-style: none;
    opacity: 1;
    padding: 0 50px 0 20px;
    text-align: left;

    -webkit-transition: -webkit-transform 300ms ease;
    transition: -webkit-transform 300ms ease;
    transition: transform 300ms ease;
    transition: transform 300ms ease, -webkit-transform 300ms ease;

    position: absolute;
    top: -50px;
    left: 0;
    z-index: 0;

    height: 50px;
    width: 100%;
    &:hover, &.active {
      background-color: #333;
      color: #fff;
    }
    &:nth-child(1) {
      -webkit-transform: translateY(2px);
      transform: translateY(2px);
      z-index: 6;
    }
    &:nth-child(2) {
      -webkit-transform: translateY(4px);
      transform: translateY(4px);
      z-index: 5;
    }
    &:nth-child(3) {
      z-index: 4;
    }
    &:nth-child(4) {
      z-index: 3;
    }
    &:nth-child(5) {
      z-index: 2;
    }
    &:nth-child(6) {
      z-index: 1;
    }
  }
}

/**/
.feaBlock {
	margin: 20px 0;
	text-align: left;
}

```
example2
```
<html>
 <form>
<fieldset>
   <label for="state">State</label>
			<select id="state" name="state"><option value="---">---</option><option value="Alabama">Alabama</option><option value="Alaska">Alaska</option><option value="Arizona">Arizona</option><option value="Arkansas">Arkansas</option><option value="California">California</option><option value="Colorado">Colorado</option><option value="Connecticut">Connecticut</option><option value="Delaware">Delaware</option><option value="District of Columbia">District of Columbia</option><option value="Florida">Florida</option><option value="Georgia">Georgia</option><option value="Guam">Guam</option><option value="Hawaii">Hawaii</option><option value="Idaho">Idaho</option><option value="Illinois">Illinois</option><option value="Indiana">Indiana</option><option value="Iowa">Iowa</option><option value="Kansas">Kansas</option><option value="Kentucky">Kentucky</option><option value="Louisiana">Louisiana</option><option value="Maine">Maine</option><option value="Maryland">Maryland</option><option value="Massachusetts">Massachusetts</option><option value="Michigan">Michigan</option><option value="Minnesota">Minnesota</option><option value="Mississippi">Mississippi</option><option value="Missouri">Missouri</option><option value="Montana">Montana</option><option value="Nebraska">Nebraska</option><option value="Nevada">Nevada</option><option value="New Hampshire">New Hampshire</option><option value="New Jersey">New Jersey</option><option value="New Mexico">New Mexico</option><option value="New York">New York</option><option value="North Carolina">North Carolina</option><option value="North Dakota">North Dakota</option><option value="Northern Marianas Islands">Northern Marianas Islands</option><option value="Ohio">Ohio</option><option value="Oklahoma">Oklahoma</option><option value="Oregon">Oregon</option><option value="Pennsylvania">Pennsylvania</option><option value="Puerto Rico">Puerto Rico</option><option value="Rhode Island">Rhode Island</option><option value="South Carolina">South Carolina</option><option value="South Dakota">South Dakota</option><option value="Tennessee">Tennessee</option><option value="Texas">Texas</option><option value="Utah">Utah</option><option value="Vermont">Vermont</option><option value="Virginia">Virginia</option><option value="Virgin Islands">Virgin Islands</option><option value="Washington">Washington</option><option value="West Virginia">West Virginia</option><option value="Wisconsin">Wisconsin</option><option value="Wyoming">Wyoming</option></select>
   </fieldset>
</form>
</html>

```
---
# small tag
The small tag defines smaller text (like copyright and other side-comments).

example
```
<!DOCTYPE html>
<html>
<body>

<h1>The small element</h1>

<p>This is some normal text.</p>
<p><small>This is some smaller text.</small></p>

</body>
</html>

```
---

# source tag
The source tag is used to specify multiple media resources for media elements, such as video, audio, and picture.

The source tag allows you to specify alternative video/audio/image files which the browser may choose from, based on browser support or viewport width. The browser will choose the first source it supports.


example1
```
<audio controls>
  <source src="http://w3tr.com/file/flut1.mp3" type="audio/mpeg">
   Tarayıcınız audio elementini desteklemiyor.
</audio>

```
example2
```
 <main class="container">
    <article class="jumbotron row">
      <div class="page-header">
        <h2>Video player</h2>
      </div>
    </article>
    <article class="well row">
      <div class="video-container col-lg-8">
        <video id='video'
               width="723px"
               height="361px"
               preload='none'
               mediagroup='myVideoGroup'
               poster="https://img00.deviantart.net/176d/i/2008/306/a/1/big_buccaneer_by_ratow.jpg">
          <source src="https://upload.wikimedia.org/wikipedia/commons/transcoded/7/79/Big_Buck_Bunny_small.ogv/Big_Buck_Bunny_small.ogv.120p.vp9.webm" type='video/webm'>
         
        </video>
        <div>
          <button id="controlsPlayPause" class="btn btn-primary" title="Play/Pause">&#9654;/&#8214;</button>
          <button id="controlsStop" class="btn btn-primary">&#9632;</button>
          <button id="controlsDecreaseVolume" class="btn btn-primary" title="Decrease volume">-</button>
          <button id="controlsMute" class="btn btn-primary" title="Mute / Unmute">&#128266;</button>
          <button id="controlsIncreaseVolume" class="btn btn-primary" title="Increase volume">+</button>
          <button id="controlsDecreaseSpeed" class="btn btn-primary" title="Decrease speed">&#9664;&#9664;</button>
          <button id="controlsIncreaseSpeed" class="btn btn-primary" title="Increase speed">&#9654;&#9654;</button>
          <button id="controlsLoop" class="btn btn-info" title="Loop">&#10561;</button>
          <button id="controlsReload" class="btn btn-success" title="Load Audio">&#8645;</button>
          <button id="controlsStepBack" class="btn btn-warning" title="Step back">&#8630;</button>
          <button id="controlsStepForward" class="btn btn-danger" title="Step forward">&#8631;</button>
        </div>
      </div>
      <div id="videoPlaylist" class="video-playlist col-lg-4"></div>
      <br/><br/>
      <progress id='progress-bar' min='0' max='100' value='0'>0% played</progress>
    </article>
    <article class="tabs-container well row video-tabs-container">
      <ul class="nav nav-tabs" role="tablist">
        <li role="presentation" class="active"><a href="#home" aria-controls="home" role="tab" data-toggle="tab">Media Events</a></li>
        <li role="presentation"><a href="#profile" aria-controls="profile" role="tab" data-toggle="tab">Media Properties</a></li>
      </ul>
      <div class="tab-content">
        <div role="tabpanel" class="tab-pane active" id="home">
          <table class="table table-striped">
            <caption>Media Events</caption>
            <tbody id='eventsTableID'>
            </tbody>
          </table>
        </div>
        <div role="tabpanel" class="tab-pane" id="profile">
          <table class="table table-striped">
            <caption>Media Properties</caption>
            <tbody id='propertiesTableID'>
            </tbody>
          </table>
        </div>
      </div>
    </article>
  </main>
  <footer class="footer">
    <p class="copyright text-center">2017 &copy; <a href="http://www.astulov.ru" target="_blank">ASTULOV.RU</a></p>
  </footer>
```
example2 CSS
```
.video-playlist {
    height: 406px;
    overflow-y: scroll;
}
.video-playlist .mt-0{
    margin: 0;
    font-size: 20px;
    line-height: 30px;
}
.video-playlist .media-object {
    width: 150px;
    height: 100px;
}
.video-tabs-container {
    height: 450px;
}

```
---
# span tag
The span tag is an inline container used to mark up a part of a text, or a part of a document.

The span tag is easily styled by CSS or manipulated with JavaScript using the class or id attribute.

The span tag is much like the div element, but div is a block-level element and span is an inline element.

example1 html
```
<ul class="colors">
  <span style="font-family: sans-serif; color:#777">Tag Color:</span>
  <li style="background: #F95;"></li>  
  <li style="background: #6AD;"></li>
  <li style="background: #E77;"></li>
  <li style="background: #6C7;"></li>
  <li style="background: #AAA;"></li>
  
</ul>


<h1 id="title">tags<span>.css</span></h1>
<label for="tag-typer">
<div id="tags">
  <span class="tag"><span class="close">&times;</span>such tage</span>
  <span class="tag"><span class="close">&times;</span>so color</span>
  <span class="tag"><span class="close">&times;</span>many type</span>
  <span class="tag"><span class="close">&times;</span>wow</span>
  <input id="tag-typer" type="text" placeholder="Add tag..."/>
  
</div>
</label>

```
example1 CSS 
```
#title{
  font:bold 48pt "Trebuchet MS";
  text-align: center;
  color: #F95;
  letter-spacing: -2px;
}
#title span{
  font-weight: normal;
  color: #BBB;
}

#tags{
  -webkit-border-radius: 10px;
  -moz-border-radius: 10px;
  border-radius: 10px;
  box-shadow: 1px 1px 4px #CCC inset;
  padding: 10px;
  width: 50%;
  background: #fafafa;
  margin: auto;
}

#tag-typer{
  outline: none;
  border: none;
  padding: 6px;
  margin: 3px;
  margin-right: -25px;
  width: 100px;
  background-color: transparent;
  font-size: 14px;
  color: #333;
}

.tag{
  display: inline-block;
  background: #F95;
  color: #FFF;
  padding: 5px 10px;
  margin:2px 2px 2px 20px;
  font: normal 16px sans-serif;
  position: relative;
  cursor: default;
  box-shadow:1px 1px 0 rgba(0,0,0,.2);
  -webkit-transform-origin:0% 50%;
  -webkit-animation: swing 1s;
  -o-animation: swing 1s;
  animation: swing 1s ;
}

.tag:before{
  content: "";
  position: absolute;
  width: 0;
  background: inherit;
  height: 10px;
  border: 10px solid #fafafa;
  border-right-color: transparent;
  -webkit-border-radius: 10px 0 0 10px;
  -moz-border-radius:10px 0 0 10px;
  border-radius:10px 0 0 10px;
  left: -20px;
  top: 0;
}

.tag:after{
  content: "";
  width: 6px;
  height: 6px;
  -webkit-border-radius: 3px;
  -moz-border-radius: 3px;
  border-radius: 3px;
  background: #FFF;
  position: absolute;
  left: -3px;
  top: 12px;
  box-shadow:inset 1px 1px 0 #CCC;
}

.tag .close{
  position: absolute;
  background: inherit;
  left: -4px;
  z-index: 3;
  visibility: hidden;
}

.tag:hover .close{
  visibility: visible;
  
}

.close:hover {
  color: rgba(0,0,0,.5);
}


.colors {
  list-style:none;
}
.colors li{
  display: inline-block;
  width:15px;
  height: 15px;
}

/* Chrome, Safari, Opera */
@-webkit-keyframes swing
{
  0%   {-webkit-transform: rotate(100deg)}
  25%  {-webkit-transform: rotate(-25deg)}
  50%  {-webkit-transform: rotate(15deg)}
  100% {-webkit-transform: rotate(0deg)}
}


@keyframes swing
{
  0%   {-webkit-transform: rotate(-200)}
  25%  {-webkit-transform: rotate(-70)}
  50%  {-webkit-transform: rotate(-185)}
  100% {-webkit-transform: rotate(-180)}
}

```
example2
```
<html>
<body>

<h1>The span element</h1>

<p>My mother has <span style="color:blue;font-weight:bold">blue</span> eyes and my father has <span style="color:darkolivegreen;font-weight:bold">dark green</span> eyes.</p>

</body>
</html>

```
---
# strong tag

The strong tag is used to define text with strong importance. The content inside is typically displayed in bold.

example
```
<html>
<body>

<h1>The strong element</h1>

<p>This text is normal.</p>

<p><strong>This text is important!</strong></p>

</body>
</html>

```
---
# style tag

The style tag is used to define style information (CSS) for a document.

Inside the style element you specify how HTML elements should render in a browser.

example
```
<!DOCTYPE html>
<html>
<head>
<style>
h1 {color:red;}
p {color:blue;}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>

```
example2
```
<!DOCTYPE html>
<html>
<head>
<style>
  h1 {color:red;}
  p {color:blue;}
</style>
<style>
  h1 {color:green;}
  p {color:pink;}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

<p>Notice that if some properties have been defined for the same selector (element) in different style sheets, the value from the last read style sheet will be used!</p>

</body>
</html>

```
---

# sub tag
The sub tag defines subscript text. Subscript text appears half a character below the normal line, and is sometimes rendered in a smaller font. Subscript text can be used for chemical formulas, like H2O.

example
```
<!DOCTYPE html>
<html>
<body>

<h1>The sub and sup elements</h1>

<p>This text contains <sub>subscript</sub> text.</p>
<p>This text contains <sup>superscript</sup> text.</p>

</body>
</html>

```
---
# summary tag

The summary tag defines a visible heading for the details element. The heading can be clicked to view/hide the details.

example1
```
<h3>The HTML5 Details/Summary tag with <a href="https://afarkas.github.io/webshim/demos/#DetailsSummary" target="_blank">webshims.lib</a> fallback.</h3>

<details class="funclass" open>
  <summary>Section 1</summary>
  <article>
    <h3>Heading</h3>
    <p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo.</p>  
  </article>
</details>

<details class="funclass">
  <summary>Section 2</summary>
  <article>
    <h3>Heading</h3>
    <p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo.</p>  
  </article>
</details>

<details class="funclass">
  <summary>Section 3</summary>
  <article>
    <h3>Heading</h3>
    <p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo.</p>  
  </article>
</details>

```
example2

```
<details>
    <summary>How does the details-tag work?</summary>
    <p>The details tag works as an interactive widget that hides / shows content.</p>
</details>
<details>
    <summary>How does the summary-tag work?</summary>
    <p>The summary tag works as the heading of the details tag. The summary will always be shown and can be clicked to show or hide the other content of the details-tag</p>
</details>
<details>
    <summary>What content can I put in the details-tag?</summary>
    <p>You can put any content you want inside of the details-tag, though the summary-tag should be the first child.</p>
</details>
<details open>
    <summary>Can I have a details-tag open by default?</summary>
    <p>Yes you can, simply add the "open" attribute to the details-tag</p>
</details>

```
---
# sup tag

The sup tag defines superscript text. Superscript text appears half a character above the normal line, and is sometimes rendered in a smaller font. Superscript text can be used for footnotes, like WWW[1].

example
```
<html>
<body>

<h1>The sub and sup elements</h1>

<p>This text contains <sub>subscript</sub> text.</p>
<p>This text contains <sup>superscript</sup> text.</p>

</body>
</html>

```
---
# svg tag 
The svg tag defines a container for SVG graphics.

SVG has several methods for drawing paths, boxes, circles, text, and graphic images.

example1
```
<html>
<body>

<h1>The svg element</h1>

<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
  Sorry, your browser does not support inline SVG.
</svg>
 
</body>
</html>

```
example2
```
<html>
<body>

<h1>The svg element</h1>

<svg width="400" height="180">
  <rect x="50" y="20" rx="20" ry="20" width="150" height="150" style="fill:red;stroke:black;stroke-width:5;opacity:0.5" />
  Sorry, your browser does not support inline SVG.
</svg>

</body>
</html>

```
---
# table tag
The table tag defines an HTML table.

An HTML table consists of one table element and one or more tr, th, and td elements.

The tr element defines a table row, the th element defines a table header, and the td element defines a table cell.

An HTML table may also include caption, colgroup, thead, tfoot, and tbody elements.

example1
```
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
}
</style>
</head>
<body>

<h1>The table element</h1>

<table>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$80</td>
  </tr>
</table>

</body>
</html>

```
example2

```
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
}

th, td {
  padding: 10px;
}
</style>
</head>
<body>

<h1>Add Padding to a Table</h1>

<table>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$80</td>
  </tr>
</table>

</body>
</html>

```
---
# tbody tag
The tbody tag is used to group the body content in an HTML table.

The tbody element is used in conjunction with the thead and tfoot elements to specify each part of a table (body, header, footer).

Browsers can use these elements to enable scrolling of the table body independently of the header and footer. Also, when printing a large table that spans multiple pages, these elements can enable the table header and footer to be printed at the top and bottom of each page.

Note: The tbody element must have one or more tr tags inside.

example1 html
```
<div class="container">
  <table class="table table-fixed">
    <thead>
      <tr>
        <th class="col-xs-3">First Name</th>
        <th class="col-xs-3">Last Name</th>
        <th class="col-xs-6">E-mail</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>

      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
      <tr>
        <td class="col-xs-3">John</td>
        <td class="col-xs-3">Doe</td>
        <td class="col-xs-6">johndoe@email.com</td>
      </tr>
    </tbody>
  </table>
</div>

```
example1 css
```
body{
  background-color: #bdc3c7;
}
.table-fixed{
  width: 100%;
  background-color: #f3f3f3;
  tbody{
    height:200px;
    overflow-y:auto;
    width: 100%;
    }
  thead,tbody,tr,td,th{
    display:block;
  }
  tbody{
    td{
      float:left;
    }
  }
  thead {
    tr{
      th{
        float:left;
       background-color: #f39c12;
       border-color:#e67e22;
      }
    }
  }
}

```
example2 html
```
<body>
 <div id="wrapper">
  <h1>Sortable Table of Search Queries</h1>
  
  <table id="keywords" cellspacing="0" cellpadding="0">
    <thead>
      <tr>
        <th><span>Keywords</span></th>
        <th><span>Impressions</span></th>
        <th><span>Clicks</span></th>
        <th><span>CTR</span></th>
        <th><span>Rank</span></th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td class="lalign">silly tshirts</td>
        <td>6,000</td>
        <td>110</td>
        <td>1.8%</td>
        <td>22.2</td>
      </tr>
      <tr>
        <td class="lalign">desktop workspace photos</td>
        <td>2,200</td>
        <td>500</td>
        <td>22%</td>
        <td>8.9</td>
      </tr>
      <tr>
        <td class="lalign">arrested development quotes</td>
        <td>13,500</td>
        <td>900</td>
        <td>6.7%</td>
        <td>12.0</td>
      </tr>
      <tr>
        <td class="lalign">popular web series</td>
        <td>8,700</td>
        <td>350</td>
        <td>4%</td>
        <td>7.0</td>
      </tr>
      <tr>
        <td class="lalign">2013 webapps</td>
        <td>9,900</td>
        <td>460</td>
        <td>4.6%</td>
        <td>11.5</td>
      </tr>
      <tr>
        <td class="lalign">ring bananaphone</td>
        <td>10,500</td>
        <td>748</td>
        <td>7.1%</td>
        <td>17.3</td>
      </tr>
    </tbody>
  </table>
 </div> 
</body>

```
example2 CSS
```
@import url('https://fonts.googleapis.com/css?family=Amarante');

html, body, div, span, applet, object, iframe, h1, h2, h3, h4, h5, h6, p, blockquote, pre, a, abbr, acronym, address, big, cite, code, del, dfn, em, img, ins, kbd, q, s, samp, small, strike, strong, sub, sup, tt, var, b, u, i, center, dl, dt, dd, ol, ul, li, fieldset, form, label, legend, table, caption, tbody, tfoot, thead, tr, th, td, article, aside, canvas, details, embed, figure, figcaption, footer, header, hgroup, menu, nav, output, ruby, section, summary, time, mark, audio, video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
  outline: none;
  -webkit-font-smoothing: antialiased;
  -webkit-text-size-adjust: 100%;
  -ms-text-size-adjust: 100%;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
html { overflow-y: scroll; }
body { 
  background: #eee url('https://i.imgur.com/eeQeRmk.png'); /* https://subtlepatterns.com/weave/ */
  font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
  font-size: 62.5%;
  line-height: 1;
  color: #585858;
  padding: 22px 10px;
  padding-bottom: 55px;
}

::selection { background: #5f74a0; color: #fff; }
::-moz-selection { background: #5f74a0; color: #fff; }
::-webkit-selection { background: #5f74a0; color: #fff; }

br { display: block; line-height: 1.6em; } 

article, aside, details, figcaption, figure, footer, header, hgroup, menu, nav, section { display: block; }
ol, ul { list-style: none; }

input, textarea { 
  -webkit-font-smoothing: antialiased;
  -webkit-text-size-adjust: 100%;
  -ms-text-size-adjust: 100%;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
  outline: none; 
}

blockquote, q { quotes: none; }
blockquote:before, blockquote:after, q:before, q:after { content: ''; content: none; }
strong, b { font-weight: bold; } 

table { border-collapse: collapse; border-spacing: 0; }
img { border: 0; max-width: 100%; }

h1 { 
  font-family: 'Amarante', Tahoma, sans-serif;
  font-weight: bold;
  font-size: 3.6em;
  line-height: 1.7em;
  margin-bottom: 10px;
  text-align: center;
}


/** page structure **/
#wrapper {
  display: block;
  width: 850px;
  background: #fff;
  margin: 0 auto;
  padding: 10px 17px;
  -webkit-box-shadow: 2px 2px 3px -1px rgba(0,0,0,0.35);
}

#keywords {
  margin: 0 auto;
  font-size: 1.2em;
  margin-bottom: 15px;
}


#keywords thead {
  cursor: pointer;
  background: #c9dff0;
}
#keywords thead tr th { 
  font-weight: bold;
  padding: 12px 30px;
  padding-left: 42px;
}
#keywords thead tr th span { 
  padding-right: 20px;
  background-repeat: no-repeat;
  background-position: 100% 100%;
}

#keywords thead tr th.headerSortUp, #keywords thead tr th.headerSortDown {
  background: #acc8dd;
}

#keywords thead tr th.headerSortUp span {
  background-image: url('https://i.imgur.com/SP99ZPJ.png');
}
#keywords thead tr th.headerSortDown span {
  background-image: url('https://i.imgur.com/RkA9MBo.png');
}


#keywords tbody tr { 
  color: #555;
}
#keywords tbody tr td {
  text-align: center;
  padding: 15px 10px;
}
#keywords tbody tr td.lalign {
  text-align: left;
}

```
---
# td tag
The td tag defines a standard data cell in an HTML table.

An HTML table has two kinds of cells:

Header cells - contains header information (created with the th element)
Data cells - contains data (created with the td element)
The text in td elements are regular and left-aligned by default.

The text in th elements are bold and centered by default.

example1 html
```
<br><h2>Testing Task List Filters</h2><hr><br>

<div class="container">
  <div class="row">
    
      <table class="table">
        <thead>
          <tr class="filters">
            <th>Baths
              <select id="assigned-user-filter" class="form-control">
                <option>0</option>
                <option>1</option>
                <option>2</option>
                <option>3</option>
                <option>4</option>
                <option>5</option>
              </select>
            </th>
            <th>Rooms
              <select id="status-filter" class="form-control">
                <option>0</option>
                <option>1</option>
                <option>2</option>
                <option>3</option>
              </select>
            </th>
            <th>Milestone
              <select id="milestone-filter" class="form-control">
                <option>None</option>
                <option>Milestone 1</option>
                <option>Milestone 2</option>
                <option>Milestone 3</option>
              </select>
            </th>
            <th>Priority
              <select id="priority-filter" class="form-control">
                <option>Any</option>
                <option>Low</option>
                <option>Medium</option>
                <option>High</option>
                <option>Urgent</option>
              </select>
            </th>
            <th>Tags
              <select id="tags-filter" class="form-control">
                <option>None</option>
                <option>Tag 1</option>
                <option>Tag 2</option>
                <option>Tag 3</option>
              </select>
            </th>
          </tr>
        </thead>
      </table>
    
    
    <div class="panel panel-primary filterable">
      <div class="panel-heading">
        <h3 class="panel-title">Tasks</h3>
        <div class="pull-right"></div>
      </div>

      
      
      
      
      <table id="task-list-tbl" class="table">
        <thead>
          <tr>
            <th>Title</th>
            <th>Created</th>
            <th>Due Date</th>
            <th>Priority</th>
            <th>Milestone</th>
            <th>Assigned User</th>
            <th>Tags</th>
          </tr>
        </thead>
        
        <tbody>
          
          <tr id="task-1"
              class="task-list-row" 
              data-task-id="1"
              data-assigned-user="3"
              data-status="2"
              data-milestone="Milestone 2"
              data-priority="Urgent"
              data-tags="Tag 2">
            <td>Task title 1</td>
            <td>01/24/2015</td>
            <td>09/24/2015</td>
            <td>3</td>
            <td>Milestone 2</td>
            <td>2</td>
            <td>Tag 2</td>
          </tr>
          
          <tr id="task-2"
              class="task-list-row" 
              data-task-id="2"
              data-assigned-user="1"
              data-status="3"
              data-milestone="Milestone 2"
              data-priority="Low"
              data-tags="Tag 1">
            <td>Task title 2</td>
            <td>03/14/2015</td>
            <td>09/18/2015</td>
            <td>1</td>
            <td>Milestone 2</td>
            <td>3</td>
            <td>Tag 1</td>
          </tr>
          
          <tr id="task-3"
              class="task-list-row" 
              data-task-id="3"
              data-assigned-user="2"
              data-status="4"
              data-milestone="Milestone 1"
              data-priority="Low"
              data-tags="Tag 3">
            <td>Task title 3</td>
            <td>11/16/2014</td>
            <td>02/29/2015</td>
            <td>2</td>
            <td>Milestone 1</td>
            <td>4</td>
            <td>Tag 3</td>
          </tr>
          
          
          <tr id="task-4"
              class="task-list-row" 
              data-task-id="4"
              data-assigned-user="1"
              data-status="1"
              data-milestone="Milestone 1"
              data-priority="High"
              data-tags="Tag 1">
            <td>Task title 4</td>
            <td>11/16/2014</td>
            <td>02/29/2015</td>
            <td>1</td>
            <td>Milestone 1</td>
            <td>1</td>
            <td>Tag 1</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</div>

```
example2
```
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
}
</style>
</head>
<body>

<h1>The td element</h1>

<p>The td element defines a cell in a table:</p>

<table>
  <tr>
    <td>Cell A</td>
    <td>Cell B</td>
  </tr>
  <tr>
    <td>Cell C</td>
    <td>Cell D</td>
  </tr>
</table>

</body>
</html>

```
---
# template tag
The template tag is used as a container to hold some HTML content hidden from the user when the page loads.

The content inside template can be rendered later with a JavaScript.

You can use the template tag if you have some HTML code you want to use over and over again, but not until you ask for it. To do this without the
 template tag, you have to create the HTML code with JavaScript to prevent the browser from rendering the code.

example1
```
<html>
<body>
<style>
.myClass {
  color: white;
  background-color: DodgerBlue;
  padding: 20px;
  text-align: center;
  margin: 10px;
}
</style>

<h1>The template Element</h1>

<p>This example fills the web page with one new div element for each item in an array.</p>
<p>The HTML code of each div element is inside the template element.</p>

<p>Click the button below to display the hidden content from the template element.</p>

<button onclick="showContent()">Show hidden content</button>

<template>
  <div class="myClass">I like: </div>
</template>

<script>
var myArr = ["Audi", "BMW", "Ford", "Honda", "Jaguar", "Nissan"];

function showContent() {
  var temp, item, a, i;
  temp = document.getElementsByTagName("template")[0];
  //get the div element from the template:
  item = temp.content.querySelector("div");
  //for each item in the array:
  for (i = 0; i < myArr.length; i++) {
    //Create a new node, based on the template:
    a = document.importNode(item, true);
    //Add data from the array:
    a.textContent += myArr[i];
    //append the new node wherever you like:
    document.body.appendChild(a);
  }
}
</script>

</body>
</html>

```
example2
```
<html>
<body>

<h1>The template Element</h1>

<p>Click the button below to display the hidden content from the template element.</p>

<button onclick="showContent()">Show hidden content</button>

<template>
  <h2>Flower</h2>
  <img src="img_white_flower.jpg" width="214" height="204">
</template>

<script>
function showContent() {
  var temp = document.getElementsByTagName("template")[0];
  var clon = temp.content.cloneNode(true);
  document.body.appendChild(clon);
}
</script>

</body>
</html>

```
---
# textarea tag
The textarea tag defines a multi-line text input control.

The textarea element is often used in a form, to collect user inputs like comments or reviews.

A text area can hold an unlimited number of characters, and the text renders in a fixed-width font (usually Courier).

The size of a text area is specified by the cols and rows attributes (or with CSS).

The name attribute is needed to reference the form data after the form is submitted (if you omit the name attribute, no data from the text area will be submitted).

The id attribute is needed to associate the text area with a label. 

example1
```
<form id="myForm">
Leave your message: <br />
<textarea name="my_textarea" rows="4" cols="50">
Enter your message here.
</textarea>
<br />
<input type="submit" value="Submit" />
</form>
<br><a href="http://www.cssinhtml.com" target="_blank">Go to CSS in HTML</a>

```
example2
```
<h1>XMLHttpRequest</h1>
<iframe style="displa:none" hidden width="700" height="315" src="https://www.youtube.com/embed/hKO3sCZy3DM" frameborder="0" allowfullscreen></iframe>
<h2>URL:</h2>
<input type="text">
<h2>Response:</h2>
  <textarea name="textarea" id="display" cols="97" rows="10"></textarea>
  <br><input type="button" value="Push me And then just touch me Till I can get my" id="work">

```
---
# tfoot tag
The tfoot tag is used to group footer content in an HTML table.

The tfoot element is used in conjunction with the thead and tbody elements to specify each part of a table (footer, header, body).

Browsers can use these elements to enable scrolling of the table body independently of the header and footer. Also, when printing a large table that spans multiple pages, these elements can enable the table header and footer to be printed at the top and bottom of each page.

Note: The tfoot element must have one or more tr tags inside.

The tfoot tag must be used in the following context: As a child of a table element, after any caption, colgroup, thead, and tbody elements.

example1
```
<table border="1">
    <thead>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
            <th>Header 3</th>
            <th>Header 4</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>This is the Body - 1</td>
            <td>This is the Body - 2</td>
            <td>This is the Body - 3</td>
            <td>This is the Body - 4</td>
        </tr>
    </tbody>
    <tfoot>
        <tr bgcolor="green">
            <td>This is Footer - 1</td>
            <td>This is Footer - 2</td>
            <td>This is Footer - 3</td>
            <td>This is Footer - 4</td>
        </tr>
    </tfoot>
</table>
<br><a href="http://www.cssinhtml.com" target="_blank">Go to CSS in HTML</a>

```
example2
```
<style>
thead {color:red;}
tbody {color:black;}
tfoot {color:pink;}

table, th, td {
    border: 1px solid black;
}
</style>
<table>
  <thead>
    <tr>
      <th>Ay</th>
      <th>Gider</th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <td>Ocak</td>
      <td>100 TL</td>
    </tr>
  </tfoot>
  <tbody>
    <tr>
      <td>Şubat</td>
      <td>50 TL</td>
    </tr>
    <tr>
      <td>Mart</td>
      <td>70TL</td>
    </tr>
  </tbody>
</table>

```
---

# th tag
The th tag defines a header cell in an HTML table.

An HTML table has two kinds of cells:

Header cells - contains header information (created with the th element)
Data cells - contains data (created with the td element)
The text in th elements are bold and centered by default.

The text in td elements are regular and left-aligned by default.

example
```
<table border="1">
	<tr>
		<th>Header 1-1</th>
		<th>Header 1-2</th>
		<th>Header 1-3</th>
		<th>Header 1-4</th>
	</tr>
	<tr>
		<td>Row 2-1</td>
		<td>Row 2-2</td>
		<td>Row 2-3</td>
		<td>Row 2-4</td>
	</tr>
</table>
<br><a href="http://www.cssinhtml.com" target="_blank">Go to CSS in HTML</a>

```
---
# thead tag
The thead tag is used to group header content in an HTML table.

The thead element is used in conjunction with the tbody and tfoot elements to specify each part of a table (header, body, footer).

Browsers can use these elements to enable scrolling of the table body independently of the header and footer. Also, when printing a large table that spans multiple pages, these elements can enable the table header and footer to be printed at the top and bottom of each page.

Note: The thead element must have one or more tr tags inside.

example
```
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
}
</style>
</head>
<body>

<h1>The thead, tbody, and tfoot elements</h1>

<table>
  <thead>
    <tr>
      <th>Month</th>
      <th>Savings</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>$100</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$80</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Sum</td>
      <td>$180</td>
    </tr>
  </tfoot>
</table>

</body>
</html>

```
---
# time tag
The time tag defines a specific time (or datetime).

The datetime attribute of this element is used translate the time into a machine-readable format so that browsers can offer to add date reminders through the user's calendar, and search engines can produce smarter search results.

example1
```
<h1>Timestamps</h1>
<p>Hover over the timestamps to see the full date:</p>
<p><time datetime="2017-04-03 08:59" title="Monday 10 April 2017 8:59am">5 minutes ago</time></p>
<p><time datetime="2017-04-03 07:59" title="Monday 10 April 2017 7:59am">1 hour ago</time></p>
<p><time datetime="2017-03-31 12:24" title="Monday 8 April 2017 12:24pm">3 days ago</time></p>
<p><time datetime="2017-03-31 12:24" title="Monday 1 April 2017 12:24pm">Apr 1, 2017</time></p>

```

example2
```
<html>
<body>

<h1>The time element</h1>

<p>Open from <time>10:00</time> to <time>21:00</time> every weekday.</p>

<p>I have a date on <time datetime="2008-02-14 20:00">Valentines day</time>.</p>

<p><b>Note:</b> The time element does not render as anything special in any of the major browsers.</p>

</body>
</html>

```
---
# title tag
The title tag defines the title of the document. The title must be text-only, and it is shown in the browser's title bar or in the page's tab.

The title tag is required in HTML documents!

The contents of a page title is very important for search engine optimization (SEO)! The page title is used by search engine algorithms to decide the order when listing pages in search results.

The title element:

defines a title in the browser toolbar
provides a title for the page when it is added to favorites
displays a title for the page in search-engine results
Here are some tips for creating good titles:

Go for a longer, descriptive title (avoid one- or two-word titles)
Search engines will display about 50-60 characters of the title, so try not to have titles longer than that
Do not use just a list of words as the title (this may reduce the page's position in search results)
So, try to make the title as accurate and meaningful as possible!

example
```
<html lang="en">
<head>
  <title>HTML Elements Reference</title>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>

```
---
# tr tag
The tr tag defines a row in an HTML table.

A tr element contains one or more th or td elements.

example
```
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
}
</style>
</head>
<body>

<h1>The tr element</h1>

<p>The tr element defines a row in a table:</p>

<table>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$80</td>
  </tr>
</table>

</body>
</html>

```
---
# track tag

The track tag specifies text tracks for audio or video elements.

This element is used to specify subtitles, caption files or other files containing text, that should be visible when the media is playing.

Tracks are formatted in WebVTT format (.vtt files).
```
<video width="320" height="240" controls>
  <track src="altyazı.vtt" kind="altyazı" srclang="tr" label="türkce">
</video>
```
---
# u tag

The u tag represents some text that is unarticulated and styled differently from normal text, such as misspelled words or proper names in Chinese text. The content inside is typically displayed with an underline. You can change this with CSS (see example below). 

example1
```
<html>
<head>
<style>
.spelling-error {
  text-decoration-line: underline;
  text-decoration-style: wavy;
  text-decoration-color: red;
}
</style>
</head>
<body>

<h1>The u element + CSS</h1>

<p>This is some <u class="spelling-error">mispeled</u> text.</p>

</body>
</html>

```
example2
```
<html>
<body>

<h1>The u element</h1>

<p>This is some <u>mispeled</u> text.</p>

</body>
</html>

```
---
# ul tag
The ul tag defines an unordered (bulleted) list.

Use the ul tag together with the li tag to create unordered lists.

Tip: Use CSS to style lists.

example
```
<html>
<body>

<h1>The ul element</h1>

<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

</body>
</html>

```
---
# var tag
The var tag is used to defines a variable in programming or in a mathematical expression. The content inside is typically displayed in italic.

example
```
<html>
<body>

<h1>The var element</h1>

<p>The area of a triangle is: 1/2 x <var>b</var> x <var>h</var>, where <var>b</var> is the base, and <var>h</var> is the vertical height.</p>

</body>
</html>

```
---
# video tag
The video tag is used to embed video content in a document, such as a movie clip or other video streams.

The video tag contains one or more source tags with different video sources. The browser will choose the first source it supports.

The text between the video and video tags will only be displayed in browsers that do not support the video element.

```
<html>
<body>

<h1>The video element</h1>

<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>

</body>
</html>

```
---
# wbr tag
The wbr (Word Break Opportunity) tag specifies where in a text it would be ok to add a line-break.

example1
```
<html>
<body>

<h1>The wbr element</h1>

<p>Try to shrink the browser window, to view how the very long word in 
the paragraph below will break:</p>

<p>This is a veryveryveryveryveryveryveryveryveryveryveryveryveryveryveryveryveryvery<wbr>longwordthatwillbreakatspecific<wbr>placeswhenthebrowserwindowisresized.</p>

<p><b>Note:</b> The wbr element is not supported in Internet Explorer 11 (or earlier).</p>

</body>
</html>

```
example2
```
<h1>wbr-Tag</h1>
<p>Donau<wbr>dampf<wbr>schiff<wbr>fahrts<wbr>kapitäns<wbr>mütze</p>
<h1>shy-Entity</h1>
<p>Donau&shy;dampf&shy;schiff&shy;fahrts&shy;kapitäns&shy;mütze</p>

```
---






