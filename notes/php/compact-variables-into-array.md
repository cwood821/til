# Compact variables into an array

The PHP `compact` function creates a key-value array based on variables in the current symbol table. Effectively, passing the name of a variable as a string will create an element in the generated array with the variable name as the key and its value as the value.

Parameter names are case sensitive.

An example from [the documentation](https://secure.php.net/manual/en/function.compact.php):

```php
$city  = "San Francisco";
$state = "CA";
$event = "SIGGRAPH";

$location_vars = array("city", "state");

$result = compact("event", "nothing_here", $location_vars);
print_r($result);
```

Would output:

```php
Array
(
    [event] => SIGGRAPH
    [city] => San Francisco
    [state] => CA
)
```

You might use this in Laravel, or other situations where you pass data to views:

```php
$firstName = "John";
$lastnNme = "Doe";

view('welcome', compact("firstName","lastName")); 
```
