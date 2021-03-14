# Editables.Js
The **Editables.Js** is a little HTML widget to manage in-place edition of text fields.

You can find a [live example](https://expandedventure.com/editablesjs/index.html) of **Editables.Js** here: [https://expandedventure.com/editablesjs/index.html](https://expandedventure.com/editablesjs/index.html)


# Getting Started
Get started in 3 simple steps.

1. Download the required libraries and stylesheets.
All these files are included in this project. You can download them from this page.

2. Include them in the <header> section of your HTML page.

```html
<script src="./javascripts/jquery-3.5.1.min.js" type="text/javascript"></script>
<script src="./javascripts/1.3.0/adminflare-demo-init.min.js" type="text/javascript"></script>
<link href="https://fonts.googleapis.com/css?family=Open+Sans:300italic,400italic,600italic,700italic,400,300,600,700" rel="stylesheet" type="text/css">	
<link href="./css/1.3.0/black-blue/bootstrap.min.css" media="all" rel="stylesheet" type="text/css" id="bootstrap-css">
<link href="./css/1.3.0/black-blue/adminflare.min.css" media="all" rel="stylesheet" type="text/css" id="adminflare-css">
	
<link rel="stylesheet" href="./editables.css">
<script src="./editables.min.js" type="text/javascript"></script>
```

3. Create a nice prefilled form.

```html
<div id='myEditable' style='position:absolute;top:50px;left:50px;'> </div>
<script>
	ctx = $('#myEditable');
	$(document).ready(function() {
		editablesJs.draw( ctx, {
			value: 'Hola Mundo!',
			placeholder: 'Write some text here.',
			onsave: function() {
				alert('Do an AJAX to save the new value here.');
			},
		});
	});
</script>
```

# Functions in Version 1.0.1
Here are listed each one of the features provided by **Editables.Js**.

## editablesJs.version()
Returns the version of this **Editables.Js** library.

## editablesJs.switchToReadOnly(ctx)
Turns off edition mode.

## editablesJs.switchToEdition(ctx)
Turns on edition mode.

## editablesJs.value(ctx)
Retrieves the value of the read-only part of the widget.

# Deployment 
The **Editables.Js** requires [**Commons.js 1.0.1**](https://github.com/leandrosardi/commonsjs), [**JQuery 3.5.1**](https://jquery.com/download/), and the **AdminFlare 1.3.0** used privately at [**ExpandedVenture**](https://expandedventure.com/expandedventure).

All the libraries are already included in this repository.

# Additional Notes
The **Editables.Js** is used at [**ExpandedVenture**](https://expandedventure.com/expandedventure) to develop different UI/UX features.

The **Editables.Js** library is just starting on Nov-2020, and more functions will be added as needed.

The **Editables.Js** library has been written following the [**W3C JavaScript Best Practices**](https://www.w3.org/community/webed/wiki/JavaScript_best_practices).

# Disclaimer
Use at your own risk. The use of the software and scripts downloaded on this site is done at your own discretion and risk and with agreement that you will be solely responsible for any damage to any computer system or loss of data that results from such activities.

# Maintainer
Leandro Daniel Sardi <leandro((dot))sardi((@))expandedventure.com>