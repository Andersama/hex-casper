# Hex Casper

The default theme for [Ghost](http://github.com/tryghost/ghost/) with a slight twist.

To download, visit the [releases](https://github.com/Andersama/hex-casper/releases) page.

## Copyright & License

Copyright (c) 2013-2016 Ghost Foundation - Released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Usage
Tags control the background color as well as orientation of posts (left / right), by default posts alternate even and odd between the two.

Color tags are:

- red
- orange
- yellow
- green
- blue
- purple
- pink
- black
- white
- (gray/grey)

Orientation tags are:

- anchor_left
- anchor_right

By default 
```css
   .main-one-page-block {
		position: relative;
		width: 100%;
		height: 50vh;
		background-size:cover;
		overflow:hidden;
   }

   .main-one-page-block img{
		position: relative;
		height: 50vh;
		background-size:cover;
		overflow:hidden;
	}
	.main-post-first {}
	.main-post-last {}
	.main-post-even, .main-post-odd {
        width:200px;
        height:50vh;
        position:relative;
        display: block;
        overflow:hidden;
        -webkit-clip-path: polygon(95% 0, 100% 50%, 95% 100%, 5% 100%, 0% 50%, 5% 0);
        clip-path: polygon(95% 0, 100% 50%, 95% 100%, 5% 100%, 0% 50%, 5% 0);
	}

	.main-post-even > article, .main-post-odd > article {
	    border-bottom: none;
	}

	.main-post-even {
		background-color: rgba(225,225,225,1);
	}
	
	.main-post-odd {
		background-color: rgba(255,255,255,1);
	}

	div.main-post-even > article {
		margin: 0rem auto 0rem 0rem;
		padding:4rem 4rem 4rem 4rem;
		background-color: rgba(255,255,255,0.90);
		-webkit-clip-path: polygon(0% 0%, 100% 0%, 100% 88%, 19% 88%, 12% 100%, 12% 88%, 0 88%);
		clip-path: polygon(0% 0%, 100% 0%, 100% 88%, 19% 88%, 12% 100%, 12% 88%, 0 88%);
	}
	
	div.main-post-odd > article{
		margin: 0rem 0rem 0rem auto;
		padding: 4rem 4rem 4rem 4rem;
		/* padding-bottom: 4rem; */
		/* background-color: rgba(225,225,225,0.8); */
		max-height: 50vh;
		Triangle Trapezoid Parallelogram Rhombus Pentagon Hexagon Heptagon Octagon Nonagon Decagon Bevel Rabbet Left arrow Right arrow Left Point Right Point Left Chevron Right Chevron Star Cross Message Close Frame Inset Custom Polygon Circle Ellipse Prefix webkit Demo Size  : polygon(0% 0%, 100% 0%, 100% 75%, 75% 75%, 75% 100%, 50% 75%, 0% 75%);
		Triangle  Trapezoid  Parallelogram  Rhombus  Pentagon  Hexagon  Heptagon  Octagon  Nonagon  Decagon  Bevel  Rabbet  Left arrow  Right arrow  Left Point  Right Point  Left Chevron  Right Chevron  Star  Cross  Message  Close  Frame  Inset  Custom Polygon  Circle  Ellipse  Prefix  webkit  Demo Size;
		-webkit-clip-path: polygon(0% 0%, 100% 0%, 100% 88%, 87% 88%, 87% 99%, 83% 88%, 0 88%);
		clip-path: polygon(0% 0%, 100% 0%, 100% 88%, 87% 88%, 87% 99%, 83% 88%, 0 88%);
	}
	
	div.main-post-odd > article > h2, div.main-post-even > article > h2 {
		font-family: "IMPACT";
		color: black;
		-webkit-text-fill-color: white; /* Will override color (regardless of order) */
		-webkit-text-stroke-width: 1px;
		-webkit-text-stroke-color: black;
	}
	
	.main-post-even img, .main-post-odd img {
		position:absolute;
        bottom:0%;
		display:block;
        min-width:25%;
		min-height:100%;
	}
	
	/*Default*/
    .main-post-even img {
		right: 0%;
    }
    .main-post-odd img {
		left: 0%;
    }
	
	.main-post-contain-image-height img {
		max-height: 100%;
		min-width: inherit;
	}
	
	.main-post-contain-image-width img {
		max-width: 100%;
		min-height: inherit;
	}
	
	.main-post-contain-image img {
		max-width: 100%;
		max-height: 100%;
	}
	
	.main-post-image-anchor-center img {
		top: 50%;
		transform: translate(0%, 50%);
		-webkit-transform: translate(0%, 50%);
	}
	
	.main-post-image-anchor-bottom img {
		bottom: 0%;
		transform: translate(0%, 0%);
		-webkit-transform: translate(0%, 0%);
	}
	
	.main-post-image-anchor-top img {
		top: 0%;
		transform: translate(0%, 0%);
		-webkit-transform: translate(0%, 0%);
	}
	
	.main-post-image-anchor-left img {
		left: 0%;
	}
	
	.main-post-image-anchor-right img {
		right: 0%;
	}
	
	div.main-post-image-anchor-right > article {
		margin: 0rem auto 0rem 0rem;
		padding:4rem 4rem 4rem 4rem;
	}
	
	div.main-post-image-anchor-left > article {
		margin: 0rem 0rem 0rem auto;
		padding:4rem 4rem 4rem 4rem;
	}
	
	.main-post-red {
		background-color: hsla(0,100%,50%,1);
	}
	
	.main-post-orange {
		background-color: hsla(25,100%,50%,1);
	}
	
	.main-post-yellow {
		background-color: hsla(50,100%,50%,1);
	}
	
	.main-post-green {
		background-color: hsla(100,100%,50%,1);
	}
	
	.main-post-blue {
		background-color: hsla(200,100%,50%,1);
	}
	
	.main-post-purple {
		/*Twitch Purple*/
		background-color: hsla(261,43%,45%,1);
	}
	
	.main-post-pink {
		background-color: hsla(300,100%,50%,1);
	}
	
	.main-post-black {
		background-color: hsla(0,0%,0%,1);
	}
	
	.main-post-gray {
		background-color: hsla(0,0%,50%,1);
	}
	
	.main-post-white {
		background-color: hsla(0,0%,100%,1);
	}
	.main-post-red > article, .main-post-orange > article, .main-post-yellow > article, .main-post-green > article, .main-post-blue > article, .main-post-purple > article, .main-post-pink > article, .main-post-black > article, .main-post-gray > article {
		background-color: rgba(255,255,255,0.9);
	}
	.main-post-white > article {
		background-color: rgba(225,225,225,0.9);
	}
```