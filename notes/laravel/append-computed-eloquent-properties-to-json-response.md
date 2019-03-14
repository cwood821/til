# Append computed Eloquent properties to JSON response

To create a computed property on an Eloquent model, define an accessor method. An example from the documentation: 

```php
public function getFullNameAttribute()
{
    return $this->first_name . " " . $this->last_name;
}
```

To append these computed properties onto JSON responses, add the `$appends` variable to the model.
```php
protected $appends = ["full_name"];
```

See further details in the [Laravel documentation](https://laravel.com/docs/5.8/eloquent-serialization).
