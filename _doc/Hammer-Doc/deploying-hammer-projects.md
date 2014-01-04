# ![](img/icon-small.png) Deploying Hammer projects

***

When you deploy a Hammer project, be sure to publish only the Build directory to your server - saving you on upload speed and deployment time.

## Publishing your entire project / Hosting with Apache

Alternatively, you can publish your entire project to your server, source files and all. This is a very useful approach for sharing projects between teams, and archiving your Hammer projects for later use.

In this case, you'll need to configure your web server to serve the site from the Build directory. You can do this in your web server's configuration.

Or, if you're using the Apache web server, simply add a `.htaccess` file on your server, in the project's root folder, to serve files from your Build folder.

	RewriteEngine on
	RewriteCond %{REQUEST_URI} !Build/
	RewriteRule (.*) /Build/$1 [L]

This ensures that your compiled, finished files are served.

***

> © 2013 Riot Ltd. All Rights Reserved - [Menu](index.md "Main menu")