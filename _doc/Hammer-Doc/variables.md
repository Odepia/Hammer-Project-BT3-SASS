# ![](img/icon-small.png) Hammer Tags

***

## Variables

With Hammer, you can set variables in your pages that you can use again and again. These can be especially useful if you need to set something that comes in from another include that you use in multiple templates.

You could use variables in Hammer to set a page title, an id attribute for the body or a class attribute in your navigation.

You create a variable using the line below:

	<!-- $title -->

You would then set the variable by using:

<!-- $title My New Title -->

In this case, we could use this `$title` variable to set a title tag in a header include for each of our pages. In `_header.html` (our head include) we would create the variable:

	<title><!-- $title --></title>

And then in our `about.html` file we could make our page title "_My About Page_" by just setting the variable like this at the top of the file:

	<!-- $title My About Page -->

You can also set a default value to be used by a variable in case a page doesn't specify a value for it:

	<!-- $title | Default Value -->

***

> © 2013 Riot Ltd. All Rights Reserved - [Menu](index.md "Main menu")