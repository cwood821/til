# Assign many variables from an array with `list` in PHP

Similar to object destructuring in JavaScript, assign variables from an array by using the `list` construct. 

```php
$simpsons = array('homer', 'marge', 'bart');

// Listing all the variables
list($homer, $marge, $bart) = $simpsons;
echo "$homer, $marge, and $bart are all characters\n";
```

See the [official documentation](https://www.php.net/manual/en/function.list.php) for more details.


