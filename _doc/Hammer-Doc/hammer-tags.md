# ![](img/icon-small.png) Hammer Tags

***

What can I do with Hammer tags?

Running your project under Hammer means you can do things you can’t normally do with standard markup and code. When any of the following features are used in your project files, Hammer will compile the markup to standard HTML inside your Build folder.

Remember, Hammer is required to use these features in development, but anyone with a web browser can view the files in the Build folder.

Some Hammer features happen automatically, some of them are called with an HTML comment formatted tag - `<!-- @keyword example -->`

***

## Clever Paths

	<img src="<!-- @path mac.png -->"/>

[Read more about Clever Paths](clever-paths.md "Read more about Clever Paths")

***

## HTML Includes

	<!-- @include _header.html -->

[Read more about includes](html-includes.md "Read more about includes")

***

## Stylesheets & JavaScript

	<!-- @stylesheet style -->
	<!-- @javascript app -->

[Read more about Stylesheet & Javascript tags](stylesheets-&-javaScript.md "Read more about Stylesheet & Javascript tags")

***

## Navigation Helpers

	<ul class="menu">
		<li><a href="<!-- @path index.html -->">Home</a></li>
		<li><a href="<!-- @path about.html -->">About</a></li>
		<li><a href="<!-- @path contact.html -->">Contact</a></li>
	</ul>

[Read more about navigation helpers](navigation-helpers.md "Read more about navigation helpers")

***

## Variables

	<!-- $title My Title -->

[Read more about variables](variables.md "Read more about variables")

***

## Todos

	<!-- @todo Fix this later -->

[Read more about todos](todos.md "Read more about todos")

***

## Image Placeholders

	<!-- @placeholder 400x300 -->

[Read more about image placeholders](image-placeholders.md "Read more about image placeholders")

***

## Automatic Reload

	<!-- @reload -->

[Read more about automatic reload](automatic-reload.md "Read more about automatic reload")

***

> © 2013 Riot Ltd. All Rights Reserved - [Menu](index.md "Main menu")