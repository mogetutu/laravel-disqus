# Disqus Bundle, by Isaak Mogetutu

A simple way to incorporate [DISQUS][1] into your Laravel application.

## Requirements

1. Laravel
2. Disqus Account

## Documentation

First get your DISQUS shortname in your account setting page.

### Usage

Add the below code into your ``application/bundles.php`` file if you want to autoload the bundle

```php
    'laravel-disqus' => array('auto' => true),
```
Add the below code into your controller.

    Bundle::start('laravel-disqus');
    $disqus = new Disqus('short_name_goes_here');
    <!-- Generated HTML is called as below -->
    $disqus->get_html();

This will embed the JavaScript which loads and displays DISQUS on your site.

## Endnote

This is the first bundle that I have made so feel free to give me any feedback/advice/guidance. Concept borrowed from
Codeigniter Disqus Spark.

[1]: http://disqus.com/
