# jQuery Stepform
jQuery StepForm is a simple plugin that converts any form into a sliding for

- each of the steps can be grouped by the class `.sf-step`
- user can slide to next step only after errors on inputs on current slide are validated
- usability for keyboard enter and tab options
- data binding for input values to be shown on confirmation screen

## Usage

Include the Javascript and CSS in the head section
```
<link rel="stylesheet" href="style.css" type="text/css" media="screen"/>
<script src="https://code.jquery.com/jquery-2.2.4.min.js" ></script>
<script type="text/javascript" src="jq.stepform.js"></script>
```

Use the html markup as below
```
<form class="stepform">
	<fieldset class="sf-step">
		<p><label class="control-label">Name</label><input class="form-control" name="name" data-validate="1"/></p>
		<p><label class="control-label">Email</label><input class="form-control" name="email" data-validate="email"/></p>
	</fieldset>
	<fieldset class="sf-step">
		<!-- input elements -->
	</fieldset>
    <fieldset class="sf-step">
        <!-- input elements -->
    </fieldset>
</form>
```

Initialize stepform
```
$(document).ready(function() {
	$(".stepform").stepform();
});
```

## API Documentation

- `data-validate` is used to validate data added to input field
 
```
data-validate="1" 		// is a mandatory feild
data-validate="5" 		// should have a minimum of 5 characters
data-validate="email"  	// should be a valid email id
```


## To Do
- Multiple data validation functions using data-validate
- Custom messages for validation
- use jQuery validate function
- onSubmit function
- parameters to customize

## License

jQuery Stepform is freely distributable under the terms of an MIT-style license.

Copyright notice and permission notice shall be included in all copies or substantial portions of the Software.

## Authors

Paresh Masade / @masade
