# ![](img/icon-small.png) Hammer Tags

***

## HTML Includes

You can include one HTML file inside another by linking to it with an `@include` tag. Just drop the `.html` extension, and include it like this:

	<!-- @include _header -->

Hammer will find your `_header.html` file, and render its content in place of the tag. If you included `_header.html` in `index.html`, when you viewed that same `index.html` file in your Build folder you’d see it would also contain the markup from `_header.html`.

You can use as many includes as you want, and you can even include files within includes. Be careful, though - don't include your templates into a loop!

***

> © 2013 Riot Ltd. All Rights Reserved - [Menu](index.md "Main menu")