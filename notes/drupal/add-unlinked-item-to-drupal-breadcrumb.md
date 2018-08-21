# Add an unlinked item to the breadcrumb in Drupal 8

Using the Drupal [Breadcrumb class](https://api.drupal.org/api/drupal/core%21lib%21Drupal%21Core%21Breadcrumb%21Breadcrumb.php/class/Breadcrumb/8.2.x), if you want to add a crumb that is not linked to anything, create a link that has the route of `<none>`.

```php
$breadcrumb->addLink(Link::createFromRoute($this->t('Current Page Title'), '<none>'));
```

This snippet is useful if you want to tack on the title of the current node, a taxonomy term name, or some other word to the end of the breadcrumb.

Found on [Drupal Stack Exchange](https://drupal.stackexchange.com/questions/192036/adding-a-non-link-element-to-the-end-of-the-breadcrumb/192040).
