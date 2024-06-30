
## modified

```php
/*
|--------------------------------------------------------------------------
| Check If The Request URI Contains /public
|--------------------------------------------------------------------------
|
| If the request URI contains /public, redirect to the root URI.
|
*/
$REQUEST_URI = "$_SERVER[REQUEST_URI]";
if (strpos($REQUEST_URI, '/public') !== false) {
    header("Location: /");
    die();
}
```
