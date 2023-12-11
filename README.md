# ConnBu

e-commerce, connects small sellers and their shops with clients by an easy and comfortable way

## Dependencies
ConnBu uses various dependencies on server-side and client-side. Those are

### Node.js 20
By the both sides, ConnBu uses modules of Node.js. You need to have Node.js 20 LTS. The modules used by ConnBu are:
+ **Material Design for Web:** Is used by UI and UX. To install you would use `npm install @material/web --save`. Visit the [Material Design for Web repository](https://github.com/material-components/material-web) to read all the documentation tah you could need. _NOTE:_ Instead inert the icon name into `<md-icon>` tag, insert the Material Icon syntax to insert an icon, at least you need to use that tag to insert icons on specific sites.
+ **Webpack:** Used as node interpreter, to _compile_ Material Design. To install you would use `npm install webpack --save`
+ **Webpack-cli:** It's just a mandatory component to webpack, used to run webpack commands, like `build`. To install you would use `npm install webpack-cli --save`

### Noto Sans
**Noto Sans** is a tipografy library distributed by Google. To use it, you would add a link tag in all necessary files into the project:

On HTML:
	
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans&display=swap" rel="stylesheet">
On CSS:

    * {
	    font-family: 'Noto Sans', sans-serif;
    }
    
    :root {
		--md-ref-typeface-brand: 'Noto Sans';
		--md-ref-typeface-plain: sans-serif;
	}
   
### Material Icons
As **Noto Sans**, **Material Icons** is an icons library distributed by Google. To use it, you would use:

On HTML:

	<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
On CSS:

	.material-symbols-outlined {
	font-variation-settings:
		'FILL' 0,
		'wght' 400,
	    'GRAD' 0,
	    'opsz' 24
	}

To use **Material Icons**, you need an `span` tag inside DOM, like the following example:

	<span class="material-symbols-outlined">
	icon_name
	</span>
Replace `icon_name` by the icon name that you need to insert.
Visit the [Material icons library](https://fonts.google.com/icons) to view the icons that you could need.

### Jquery 3.7.1
Only used to simplify work with JavaScript on client-side. To use it, insert on HTML head:

	<script src="https://code.jquery.com/jquery-3.7.1.js" integrity="sha256-eKhayi8LEQwp4NKxN+CfCh+3qOVUtJn3QNZ0TciWLP4=" crossorigin="anonymous"></script>