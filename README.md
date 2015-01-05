An Intro to Scalable Vector Graphics
====================================

Over Christmas, I decided to learn some of the basics of Scalable Vector Graphics (SVG).  The below offers the basic outline of a talk I subsequently gave at Makers Academy on the topic.  This is meant to serve as a very basic introduction to SVG and scratch the surface of some of its key selling points.  My presentation is best consumed with a basic grasp of jQuery, CSS3, and HTML.  The files are hosted here on Heroku.

---------- add all links.
---------- delete needless files in respository.


###What Is A Scalable Vector Graphic?  Why Should You Care?
SVG graphics are lossless.  You can scale them up as much as you like without suffering any degradation in quality and they are typically small in file size too.  Oh, and just one more thing.. with SVG, you have the ability to dynamically alter and control internal elements, shapes and attributes of your graphics.  You can change strokes, alter shapes, adjust fills in your browser on the fly and take advantage of powerful animation libraries.  Put together, these features render SVG perfect for the web, well-supported, well-equipped for responsive design, great for mobile, and fantastic for creativity.  Chrome supports SVG out of the box.

###Example #1 : How Could You Get Started With SVG Today?
The front-page of my presentation here uses just one single 4kb SVG file.  The sliding animation is simply controlled via CSS but this illustrates quite simply some of the beauty of SVG and its crisp, smooth, lossless characteristics.  You can contrast this with an equivalent page using a small 200px 4kb GIF file I found here.  008 link.  Thus, what this means for you today is that where you are presented with a choice between using an SVG file or another in perhaps GIF or JPG format, you may find SVG more flexible, placing you better for customers on anything from mobile to 5k retina-like screens.  And if you do find an SVG file, don't be afraid to play with it a touch.

###Example #2 : The Next Step : Beneath The Bonnet Of SVG 
Assuming you hold an SVG file, you may decide that you would like to customise it on the fly.  For example, you may like to modify small elements of the graphic and style the fill or stroke of an element in response to a jQuery event such as a click or mouseover.  To do this, you need to understand how SVG files are put together, therefore let us look at an example.  

All SVG files are simply collections of shapes and lines or paths.  The '0' in the '007' logo could be considered as a couple of rotated ellipses or even closed path elements while the crocodile copied below could be seen as a structure of polygons.  The elements that make up SVG images can take a stroke and fill and are described in mark-up very similar to HTML.  Below is the SVG code that describes the computer graphic copied further beneath.  If you were to assign the ```rect``` and ```polygon``` elements individual ```id``` attributes and remove their currently assigned ```fill``` attributes, you would now be in a position to style the computer via a CSS file. 

[It is through this logic that my opening "007" page can easily take a more minimalist style]().  [Further examples with the Leeds United FC logo can also be found here.]()  The Yorkshire Rose pops out and rotates on mouseover, the core badge fill takes a patterned fill defined by the SVG diagonal box on the left-hand-side of the page, the chevrons and text fade and take a stroke, and the "l" letter flies in completing the graphic on page load.  [And if you prefer cats, try this.](http://codepen.io/miukimiu/full/Igouf/)

```html

<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
	 viewBox="0 0 648 500" enable-background="new 0 0 648 500" xml:space="preserve">
<g>
	<rect x="81.479" y="30.406" fill="#989898" width="485.58" height="345.509"/>
	<polygon fill="#818181" points="81.479,375.915 6.775,450.619 641.765,450.619 567.06,375.915 	"/>
	<polygon fill="#676767" points="620.983,469.296 23.345,469.296 4.669,450.619 639.659,450.619 	"/>
	<rect x="100.156" y="77.096" fill="#0DAE8A" width="448.228" height="261.466"/>
</g>
</svg>

```


![Computer](https://github.com/benhutchinson/SVG/blob/master/public/img/computer.png)

![SVG Snap Logo](https://github.com/benhutchinson/SVG/blob/master/public/img/crocodile.png)


###Example #3 : Working With A Library
Given that all SVG files are shapes and paths that can be configured and styled or mathematically altered, it shouldn't be too much of a surprise to learn that animation libraries exist.  A nice one that I found is called Walkway.js which [animates wireframe drawings of PS4 consoles here](http://www.connoratherton.com/walkway) and [here](http://www.polygon.com/a/ps4-review) and can used "to animate SVG images consisting of line, path, and polyline elements."  The author's code [is stored on Github](https://github.com/ConnorAtherton/walkway).  I was able to use this library together with camera graphic I found on Google Images below, and use this to [animate some of the sign-in pages on my Instagram project.](http://beninst.herokuapp.com/users/sign_up)


![Camera](https://github.com/benhutchinson/SVG/blob/master/public/img/camera.png)

###Concluding Thoughts & More Inspiring Examples
Learning about SVG very much reminds me of Adobe Flash.  The more you learn how to use it, the more the boundaries between the web and graphics design appear to blur.  Modern browsers appear to be quite powerful rendering agents, almost serving as an extension of a graphic software's canvas.  This said, I think it is important to stress that SVG offers more than just animation.  For example, [D3.js is a JavaScript library for manipulating documents based on data](http://d3js.org) and one of the next libraries I am personally keen to explore.  


If you would just like to s




To use it well and to create illustrations of your own, clearly a mastery of Adobe Illustrator or the free version 


It seems exceptionally powerful when use

http://snapsvg.io/demos/

http://thegraphicalweb.com/


Examples can be found

creating graphics, use well w illustrator

limits - ie. want to access elements, but more precise shaping etc and defining of elements better in a graphics package
check on smaller mac
heroku host
tidy up a bit more
rough examples cna't cover - clip, mask more animations
the examples in the adobe library
conclusion, remidns me of flash a bit.




###So SVG Is Great But What Is Is Not?
- SVG files are not photos...
- The more I learned about the different ways to play with and animate SVG files, the more I appreciated the ease of CSS.  There are some [good tutorials on some CSS transition properties here](http://www.atozcss.com/episodes/) that even touch on some basic 3D transformations such as ```perspective``` for example.
- It is good to have an understanding of how SVG files are composed mathematically, their co-ordinate grid, and how they can be controlled, but clearly for advanced illustrations, using dedicated graphics software such as Adobe Illustrator will be more intuitive.  [Adobe's Project Parfait](http://www.adobe.com/uk/creativecloud/extract.html) also offers insight into how tightly graphics software is being integrated into the web development process.
- More [advanced blending-mode properties](http://webplatform.adobe.com/) seem to be in development.

###Where To Learn More

###Resources & Tutorials
- [Caniuse.com](http://www.caniuse.com) is a useful web-site if you want to assess a feature's cross-browser functionality.  This is important as the graphical web is continually evolving.
- [If you are new to graphics, Adobe provide a bit of an overview of some of the different image types that exist and the difference between vector and raster image files](https://helpx.adobe.com/illustrator/how-to/illustrator-bitmap-vs-vector.html)
- The [Vox Media Xbox One Review](http://product.voxmedia.com/2013/11/25/5426880/polygon-feature-design-svg-animations-for-fun-and-profit) is an interesting SVG case study and a real-world example showing how a vector illustration is put together in Adobe Illustrator before finding its way on to the web and being animated, and I think it was the inspiration for Walkway.js
- A Simple Fun Tutorial: [Animate SVG With CSS](https://jonsuh.com/blog/animate-svg-with-css/)
- [CSS Tricks: A Compendium Of SVG Information](http://css-tricks.com/mega-list-svg-information/)
- [MDN's SVG Tutorial](https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial) is fairly thorough if you would like to know a little more about SVG under the hood.
- [Jenkov's SVG Tutorial](http://tutorials.jenkov.com/svg/index.html).  37 topics.  Pick the ones that interest you.  It is quite clear.
- [An Online SVG File Converter](http://image.online-convert.com/convert-to-svg).  Try it and see if it works.  I have used it successfully with some png files that appear loss-less or hold some transparency.  Clearly a more optimal solution would be to use a dedicated vector package such as Adobe Illustrator.
- [Inkscape](https://inkscape.org/en/) is a free vector illustration package.  I used it to open SVG files that I found and was able to "ungroup" shapes that were bound together in groups.  I could then use the software to assign an ```id``` to a shape.  This is much easier than guessing from within an SVG markup that is littered with numbers.

###Well-Known Javascript Libraries
- [Snap](http://snapsvg.io) : linked to Adobe and aiming to take advantage of the very latest browsers
- [Raphaël](http://raphaeljs.com/) : included in Snap.  Less advanced but more cross-browser compatibility.

###Technologies
- SVG
- CSS
- jQuery
- Inkscape
- Node.js, Express Server, EJS Templating