## Templates
:relaxed: Quick web front-end

## Think about
Web development can be boring with much environments! The web-components concept comes with a price, and the browser manage it, we chose resolve our issues of scope before the page render, on the server!

## Boilerplate taken seriously
You can't wasting your time doing things that you already did 100000000000 times. 
Checkout our wiki: https://github.com/objectbody/templates/wiki

### Example

#### Input

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
	<meta charset="UTF-8">
	<title>Example!</title>
</head>
<body>
	
	<main>
		Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
		tempor incididunt ut labore et dolore magna aliqua.
	</main>

	<style tpl="someStyle" tpl-style>
		body { background: red; }
	</style>

	<script tpl="someScript" tpl-script>
		console.log('hi')
	</script>

	<script tpl="someFramework" src="//cdn.com/framework.min.js" tpl-require></script>
	<link tpl="someLibrary" href="//cdn.com/library.min.css" tpl-require>

</body>
</html>
```

#### Output

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
	<meta charset="UTF-8">
	<title>Example!</title>
	<link href="//cdn.com/library.min.css">
	<style type="text/css">body{background:red}</style>
</head>
<body>
	<main>
		Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
		tempor incididunt ut labore et dolore magna aliqua.
	</main>
	<script src="//cdn.com/framework.min.js"></script>
	<script type="text/javascript">console.log('hi')</script>
</body>
</html>
```
