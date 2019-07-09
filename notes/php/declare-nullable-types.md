# Declare Nullable Types

Since PHP 7.1, you can declare nullable types by prefixing normal types with a question mark. 

For example:

```php
function answer(): ?int  {
    return null; //ok
}
```

The example above comes directly from the [RFC](https://wiki.php.net/rfc/nullable_types). Also, see this [Stack Overflow conversation](https://stackoverflow.com/questions/33608821/nullable-return-types-in-php7). 

