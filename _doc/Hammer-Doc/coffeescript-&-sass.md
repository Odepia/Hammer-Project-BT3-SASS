# ![](img/icon-small.png) Language Support

***

## SASS & CoffeeScript

Hammer will automatically compile `.coffee` files to `.js` files and `.scss` and `.sass` files to `.css` files. You don’t need to anything to make this happen, Hammer handles it for you.

	<!-- @javascript application -->

Because Hammer finds application.coffee, and it knows about this filetype, it will convert this link to:

	<script src="assets/js/application.js" type="text/javascript">

### SASS Mixins

Hammer includes **[Bourbon's set of SASS mix-ins](http://thoughtbot.com/bourbon/ "Bourbon's set of SASS mix-ins")** for use in your app. Whether you're using SCSS or SASS, mix-ins are a useful trick for avoiding vendor prefixes in your code.

	.animate-me {
	    @include transition( all 0.8s );
	    @include transform( rotate(45deg) skew(20deg, 30deg) );
	}

You don't have to use mix-ins, but they're a great way of writing clean, concise code. A full list of the mix-ins included is available on the **[Bourbon site](http://thoughtbot.com/bourbon/ "Bourbon site")**.

Ref: [CoffeeScript](http://coffeescript.org/ "CoffeeScript") - [SASS](http://sass-lang.com/ "SASS")

***

> © 2013 Riot Ltd. All Rights Reserved - [Menu](index.md "Main menu")