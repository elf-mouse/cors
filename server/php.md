# CORS on PHP

If you don't have access to configure Apache, you can still send the header from a PHP script. It's a case of adding the following to your PHP scripts:

```php
<?php
header("Access-Control-Allow-Origin: *");
```

> Note: as with all uses of the PHP [header function](https://php.net/manual/en/function.header.php), this must be before any output has been sent from the server.
