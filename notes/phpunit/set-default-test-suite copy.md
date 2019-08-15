# Set constant in phpunit.xml  

To make a PHP constant available in a test suite in PHPUnit, you can add it to the `phpunit.xml` file. 

Example:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<phpunit>
    <php>
        <const name="DEBUG" value="FALSE"/>
    </php>

    <testsuites>
        <testsuite name="unit">
            <directory suffix="Test.php">tests/Unit</directory>
        </testsuite>
    </testsuites>
</phpunit>

With that config, you'll be able to reference `DEBUG` in your PHP code.

Hat tip to this [Stack Overflow discussion](https://stackoverflow.com/questions/3906968/global-constants-in-phpunit). 


