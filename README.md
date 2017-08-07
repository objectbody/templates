## Templates
:relaxed: Quick web front-end

### Some Input

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

### Some Output

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
