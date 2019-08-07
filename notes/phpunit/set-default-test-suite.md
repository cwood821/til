# Set default test suite in PHPUnit 

To set a default test suite in PHPUnit, add the defaultTestSuite attribute to the phpunit tag in the `phpunit.xml file`. Be sure its value corresponds to a test suite later in the file.

Example:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<phpunit
        defaultTestSuite="unit"
 >
    <testsuites>
        <testsuite name="unit">
            <directory suffix="Test.php">tests/Unit</directory>
        </testsuite>
    </testsuites>
</phpunit>
```

Now, to run the default test suite, just run `phpunit` without arguments:

```bash
phpunit
```

See the this [Stack Overflow discussion](https://stackoverflow.com/questions/37820193/running-a-single-testsuite-by-default-in-phpunit) for discussion. 


