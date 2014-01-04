# ![](img/icon-small.png) Tips & Tricks

***

## 404 pages

Building a 404 page is an important detail for any site. However, Hammer's special Clever Paths make it tricky to host a single static page anywhere on your site. If you build your 404.html page in the root of your project, assets links will point to relative paths, instead of absolute ones. Oh no!

Fortunately, there's a way around this. Simply add this tag to the `<head>` element of your 404.html page:

	<base href="/">

This will make your asset paths behave as though they were absolute paths from the site's root. Nice!

Note: You'll need to run your site from a hostname for this to work properly. For example, `http://mysite.dev/` or `http://mysite.com/`. By default, Hammer uses `file:///` URLS, which do not play nicely with `<base>` tags.

***

> © 2013 Riot Ltd. All Rights Reserved - [Menu](index.md "Main menu")