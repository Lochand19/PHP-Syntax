# PHP Syntax Guide
### Lochlan Dorman

 ## 1. PHP Comments:
PHP comments are not visible to the user on a webpage but are visible for the coder in the actual php file. These are useful for labeling important information or instructions in the file that may be forgotten and needed at a later date. They are also useful for formatting files. They can be single or multiline.
> 
	<?php
	//This is a single line comment created with two foreward slashes.
	/* This is a
	multiline comment 
	signified by the foreward slash
	and star at beginning and
	end */
	?>

## 2.  PHP Variables:
PHP variable can be used to store strings, numbers and other values. PHP variables automatically convert the variable to the proper data type making it easier than other code syntaxes. They are declared using a $ infront of the variable name and an = to signify the value.

> 
	<?php
	$variable1 = "pizza"; //here is a string variable with "" around the string.
	$variable2 = 25; //here is a number variable

	echo $variable1; //this will output the value for variable1 which is 'pizza'.
	echo $variable2; //this will output the value for variable2 which is '25'.
	?>

## 3. PHP Echo and Print:
Echo and print are used to output data onto the users screen. Echo is faster than print and can have multiple parameters. Print is useful in expressions because the return value is always 1 and it can opnly accept one argument.

- ### Echo
> 
	<?php
	echo "This is a single string"; //output: This is a single string
	echo "String with more than one ", "parameter"; //output: String with more than one parameter
	?>

- ### Print
> 
	<?php
	print "Hello there"; //output: hello there
	?>

## 4. PHP Data Types:
PHP has 8 different data types. These consist of intergers, floats, strings, booleans, arrays, objects, resources and NULL. For information on intergers or floats, refer to PHP numbers. For information on strings, refer to PHP strings. for information on arrays, refer to PHP arrays.

- ### Booleans
Booleans are a PHP datatype that can be either 'true' or 'false'.
> 
	<?php
	$variable1 = true; //this assigns the variable 'variable1' to a value of true
	?>

- ### Objects
In PHP, objects can be created similarly to javascript. An object will have a name and some form of property(s).
> 
	<?php
	$car = (object) [
		'horsepower' => '120',
		'color' => 'blue',
	];
	?>

- ### Resources
Resources are an external resource referenced by PHP.
>
	<?php
	<form action="php_table.php" method="POST"> //references to an external file called "php_table.php"
	?>

- ### Null
PHP NULL references a value of null, this is a special value.
>
	<?php
	$value = NULL; //the $value is equal to NULL
	?>


## 5. PHP Strings:
Strings are a combination of letters numbers or special characters enclosed in single quotation marks. 

> 
	<?php
	#a_string = 'hello there';
	echo '$a_string'; //displays 'hello there'
	?>

## 6. PHP Numbers:
Intergers are whole numbers where as floats are numbers with a decimal.

- ### Intergers
> 
	<?php
	$interger1 = 126; //this is a whole number meaning it is an interger
	?>

- ### Floats
> 
	<?php
	$float1 = 12.56; //this is a number with a decimal meaning it is a float
	?>

## 7. PHP Constants:
Constants in PHP are variables that can only be defined once, and can not change.
> 
	<?php
	define('AUTHOR', 'Lochlan Dorman');
	echo AUTHOR; //This will display the defined constant: 'Lochlan Dorman'.
	?>

## 8. PHP Operators:
Operators are used to perform operations on defined values and variables in PHP. These include + (addition) - (subtraction) * (multiplication) / (division) % (modulus) and ** (exponents).
> 
	<?php
	$value1 = 10;
	$value2 = 20;
	$value3 = $value1 + $value2;
	echo $value3; //displays 30
	?>

## 9. PHP If & Else & Elseif:
PHP IF, Else and Else IF statements are similar to javascript in that they check on a condition, and then execute some code. The if statement checks is a condition is true then executes code. If the condition is not met then the code is skipped. The Else statement comes after an If statement in the same block and will execute when the condition on the If statement is not met. The Else If statement similarly to the Else statement will execute after an If statement condition is not met but it also has a new condition that must be met before the code can be executed. 

>
	<?php
	$condition = 20; //variable is set
	if ($condition = 20) { //if statement checks the condition
	echo "I like that number; //executes code if condition is met
	} else {
	echo "I don't like that number"; //else statement executes code if the original if statement is not met
	}
	?>

## 10. PHP Functions:
PHP function are very similar to javascript function in that the function must be declared, and then called.
>
	<php
	function myfunction(){
	echo "Hello There"; //function is declared
	}
	myfunction(); //function is called and displays "Hello There"
	?>

## 11. PHP Arrays:
Arrays in PHP can hold more than one value at a time.
> 
	<?php
	$car_type = array('honda','subaru','ford'); //this array ($car_type) holds 3 different car types.
	?>

## 12. PHP Loops:
There are 4 different types of PHP loops. These are the while loop, the do loop, the for loop and the for each loop. These generally loop through conditions and execute some sort of code depending on the condition.
>
	<?php
	for($i=1; $i<=20; $i++){ //condition for loop
    echo $i . " "; //code to be executed (will display 1 through 20 then stop)
	}
	?>
