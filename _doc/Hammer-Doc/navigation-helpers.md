# ![](img/icon-small.png) Hammer Tags

***

## Navigation Helpers

Traditional navigation menus tend to work the same way, so we’ve standardized this in Hammer and take care of the dynamic aspects for you.

When Hammer sees an href that’s linking to the page it’s on, it adds a class of ‘current’ to the anchor tag and to be extra helpful, if the anchor tag is wrapped in a list item, the list item also gets that ‘current’ class.

	<ul class="menu">
	  <li><a href="<!-- @path index.html -->">Home</a></li>
	  <li><a href="<!-- @path about.html -->">About</a></li>
	  <li><a href="<!-- @path contact.html -->">Contact</a></li>
	</ul>

In the example below we’re looking at the about.html file in our Build folder:

	<ul class="menu">
	  <li><a href="index.html">Home</a></li>
	  <li class="current"><a href="about.html" class="current">About</a></li>
	  <li><a href="contact.html">Contact</a></li>
	</ul>

To help out with nested navigation, links pointing to the current directory's, or to a parent directory's index.html file are given the class 'current-parent'. This means that no matter which page you're in, your primary navigation can always have a 'current-parent' class if you're in that folder. For instance, if you're inside docs/info.html, then any links to docs/index.html will have the 'current-parent' class.

	<ul class="menu">
	  <li><a href="<!-- @path about/index.html -->">Home</a></li>
	  <li><a href="<!-- @path about/team.html -->">Team</a></li>
	  <li><a href="<!-- @path about/contact.html -->">Contact</a></li>
	</ul>

In the example below we’re looking at the about.html file in our Build folder:

	<ul class="menu">
	  <li><a class="current-parent" href="about/index.html">Home</a></li>
	  <li class="current"><a href="about/team.html" class="current">About</a></li>
	  <li><a href="contact.html">Contact</a></li>
	</ul>

***

> © 2013 Riot Ltd. All Rights Reserved - [Menu](index.md "Main menu")