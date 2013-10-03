Transliterate.php
=================

A PHP class for transliteration

Simple examples:

```php
echo Transliterate::to_ascii('Фёдор Михайлович Достоевский', 'russian');
// Result: Fedor Mihajlovich Dostoevskij

echo Transliterate::to_ascii('Фьодор Михайлович Достоевски', 'bulgarian');
// Result: Fyodor Mihaylovitch Dostoevski
```

Example on CodeIgniter framework, making a slug for permalink creation:

```php
$product_name = 'Авторско колие с естествен камък тюркоаз';

$product_name_ascii = Transliterate::to_ascii($product_name);
// Result: Avtorsko kolie s estestven kamak tyurkoaz

$product_slug = url_title($product_name_ascii, '-', true);
echo $product_slug;
// Result: avtorsko-kolie-s-estestven-kamak-tyurkoaz
```

Author: Ivan Tcholakov <ivantcholakov@gmail.com>, 2012-2013

License: The MIT License
