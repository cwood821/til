# Use data providers to provide variations on input

Data providers are a concise way to arrange variations on input data for a test. To use one, create a function that returns an array of data. Next, annotate a test with `dataProvider` and take in the data as a parameter. 

```php
// Assumes inside PHPUnit test class

public function myProvider() {
  return [1, 2, 3];
}
    
/**
* @dataProvider myProvider
*/
public function testDataAreNumbers($num) {
  $this->assertEquals(true, is_numeric($num));
}

```

This will run the test with each data value. 

Read [the documentation](https://phpunit.readthedocs.io/en/8.4/writing-tests-for-phpunit.html#writing-tests-for-phpunit-data-providers-examples-datatest-php). Tighten has a nice [blog post](https://tighten.co/blog/tidying-up-your-phpunit-tests-with-data-providers).  
