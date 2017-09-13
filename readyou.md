[![enter image description here][1]][1]


[![enter image description here][2]][2]


**app\views\index.js**

    <!DOCTYPE html>
    <html>
    <head>
    	<title><%= title %></title>
    	<base href="/">
    </head>
    <body>
    	<mean-app>
    		<h1>Loading...</h1>
    	</mean-app>
    	
    	<script type="text/javascript">
    		window.user = <%- user || 'null' %>;
    	</script>
    	
    	<script src="lib/core-js/client/shim.min.js"></script>
    	<script src="lib/zone.js/dist/zone.js"></script>
    	<script src="lib/reflect-metadata/Reflect.js"></script>
    	<script src="lib/systemjs/dist/system.js"></script>
    	
    	<script src="systemjs.config.js"></script>
    	<script>
    		System.import('app').catch(function(err){ console.error(err); });
    	</script>
    </body>
    </html>


[Chapter07 on GitHub][3]


  [1]: https://i.stack.imgur.com/yFg3k.png
  [2]: https://i.stack.imgur.com/h1qQ8.png
  [3]: https://github.com/TurtleWolf/Chapter07
