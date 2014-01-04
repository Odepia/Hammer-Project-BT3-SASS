# ![](img/icon-small.png) Hammer Tags

***

Stylesheets & JavaScript

Hammer does some extra things for linking to your stylesheet and javascript files. Instead of writing out the full tags to reference these files, you can do the following:

	<!-- @stylesheet style -->
	<!-- @javascript app -->

When these are rendered out in your Build folder they will become:

	<link rel="stylesheet" href="stylesheets/style.css" />
	<script src="assets/js/app.js" type="text/javascript"></script>

You can reference SASS and CoffeeScript files in exactly the same way, just by filename, and they'll be rendered out as stylesheet and javascript tags.

If you have multiple stylesheets in your project, you could use a wildcard with the tag to link to them all:

	<!-- @stylesheet reset -->
	<!-- @stylesheet assets/css/* -->

This renders in your Build as:

	<link rel="stylesheet" href="assets/css/reset.css"/>
	<link rel="stylesheet" href="assets/css/style.css"  />
	<link rel="stylesheet" href="assets/css/mobile.css"  />

Remember to specify by name the files you need first, (eg. a reset css file or a library javascript file) as in the example above. Hammer knows you don't want `reset.css` to be included twice so the * rule will ignore it because it's already been specified.

You can even reference multiple files:

	<!-- @stylesheet reset normalize buttons style -->

In development mode, Hammer links your page to every stylesheet or script. Then, when you're ready to go live, just switch to **[Optimize mode](optimized-mode.md "Optimize mode")**, and Hammer will compress them all into one file.

***

> © 2013 Riot Ltd. All Rights Reserved - [Menu](index.md "Main menu")