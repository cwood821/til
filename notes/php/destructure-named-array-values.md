# Destructure named array values in PHP

To destructure a value value from a named array, use this syntax:

```php
$arr = ["ID" => 3];
["ID" => $id] = $arr; 
echo $id; // 3
```

See this post for [variations](https://supunkavinda.blog/php-list). Also, see [`extract`](https://www.php.net/manual/en/function.extract.php).
