Transliterate.php
=================

A PHP class for transliteration

Examples:

```php
echo Transliterate::to_ascii('Фёдор Михайлович Достоевский', 'russian');
// Result: Fedor Mihajlovich Dostoevskij

echo Transliterate::to_ascii('Фьодор Михайлович Достоевски', 'bulgarian');
// Result: Fyodor Mihaylovitch Dostoevski
```

Author: Ivan Tcholakov <ivantcholakov@gmail.com>, 2012-2013

License: The MIT License
