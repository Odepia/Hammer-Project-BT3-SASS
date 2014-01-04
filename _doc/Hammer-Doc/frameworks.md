# ![](img/icon-small.png) Tips & Tricks

***

## Frameworks

### Bourbon Neat and Hammer

If you're using the fantastic ***[Bourbon Neat](http://neat.bourbon.io/ "Bourbon Neat")** framework with Hammer, you'll need to **[download the Neat code](https://github.com/thoughtbot/neat/archive/master.zip "Download the Neat code")** from the **[Neat GitHub repository](https://github.com/thoughtbot/neat "Neat GitHub repository")**. The SCSS files for Neat are located inside the app/assets/stylesheets directory.

To use Neat in your project, simply copy the contents of _app/assets/stylesheets_ into a folder in your project. Then just use `@import "neat";` in your SCSS or Sass files to use Neat.

***

### ZURB Foundation and Hammer

If you're working with **[ZURB's Foundation framework](http://foundation.zurb.com/ "ZURB's Foundation framework")**, you'll need to grab the **[Standalone Foundation files from GitHub](https://github.com/zurb/foundation/tree/scss-standalone "Standalone Foundation files from GitHub")**.

Simply include the Foundation files in your project, include them in your SCSS files with `@include "foundation/foundation"` and you're good to go!

***

### Compass and Hammer

Hammer doesn't support Compass, or compass-based CSS frameworks. There are many reasons why this is the best choice for us, and for you.

For more information on why we don't support this particular framework, please read our blog post, **["Why we don't support Compass"](http://hammerformac.com/news/compass.html "Why we don't support Compass")**.

If the Compass-based framework you're using has a standalone option (like **[ZURB Foundation](https://github.com/zurb/foundation/tree/scss-standalone "ZURB Foundation")**) that doesn't require Compass, you should be able to use it just fine!

***

> © 2013 Riot Ltd. All Rights Reserved - [Menu](index.md "Main menu")