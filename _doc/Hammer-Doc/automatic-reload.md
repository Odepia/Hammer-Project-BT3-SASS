# ![](img/icon-small.png) Hammer Tags

***

## Automatic Reload

When you’re building your HTML and you’re writing your CSS you want to be able to quickly and reliably view the changes as they happen. Just use the `@reload` tag in your `<head>` element.

	<!-- @reload -->

Hammer automatically refreshes your page whenever it rebuilds. Since it builds every time you save, it's a great way of viewing your changes as you write code.

Technicaly, this tag adds the following code into the HTML page:

        <!-- Hammer reload -->
          <script>
            setInterval(function(){
              try {
                if(typeof ws != 'undefined' && ws.readyState == 1){return true;}
                ws = new WebSocket('ws://'+(location.host || 'localhost').split(':')[0]+':35353')
                ws.onopen = function(){ws.onclose = function(){document.location.reload()}}
                ws.onmessage = function(){
                  var links = document.getElementsByTagName('link');
                    for (var i = 0; i < links.length;i++) {
                    var link = links[i];
                    if (link.rel === 'stylesheet' && !link.href.match(/typekit/)) {
                      href = link.href.replace(/((&|\?)hammer=)[^&]+/,'');
                      link.href = href + (href.indexOf('?')>=0?'&':'?') + 'hammer='+(new Date().valueOf());
                    }
                  }
                }
              }catch(e){}
            }, 1000)
          </script>
        <!-- /Hammer reload -->

***

> © 2013 Riot Ltd. All Rights Reserved - [Menu](index.md "Main menu")