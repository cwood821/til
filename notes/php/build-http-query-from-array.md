# Build HTTP query from an array in PHP

To build an HTTP query string in PHP from an array, use the `http_build_query` function.

```php
$data = [ 
    'firstname' => 'bob',
    'lastname' => 'barker'
];

echo http_build_query($data) . "\n";
```

This will output:
```
firstname=bob&lastname=barker
```

It will also work with an object, but only use public properties. See [the documentation](https://secure.php.net/manual/en/function.http-build-query.php) for further details. Notably, it is possible to change the encoding type based on two different RFC's to encode spaces as `+` or `%20`.
