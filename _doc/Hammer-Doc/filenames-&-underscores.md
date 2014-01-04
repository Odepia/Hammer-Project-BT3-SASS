# ![](img/icon-small.png) Filenames in Hammer

***


## How do filenames work in Hammer?

In a Hammer project, you create all your templates in your project folder. Inside, Hammer creates a Build directory, and processes all of your files into it. That means, when you're ready, you can publish just the Build directory to your server.

## Underscores

If a Hammer file starts with an underscore, it's treated as an included file. That means it isn't compiled directly into the Build directory, but can be included inside other files.

That's why you should use filenames like `_header.html` for included files. Otherwise, if you try to use a variable in `header.html` without defining it in the same file, `header.html` will fail to build.

The same goes for SASS & SCSS files - _style.scss won't be compiled into Build/_style.css.


***

> © 2013 Riot Ltd. All Rights Reserved - [Menu](index.md "Main menu")