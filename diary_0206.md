# Diary 02.06.2020


* session information is stored within the browser
* for forms that allow a file upload, you need to add ```enctype="multipart/form-data"``` next to ```action="" and method=""```
* the keyword ```pathinfo``` gives information about a file path. you can get several different infos from the path:
  * ```PATHINFO_DIRNAME``` 
  * ```PATHINFO_BASENAME``` 
  * ```PATHINFO_EXTENSION``` 
  * ```PATHINFO_FILENAME``` 
```php
<?php
$path_parts = pathinfo('/www/htdocs/inc/lib.inc.php');

echo $path_parts['dirname'], "\n";  // '/www/htdocs/inc'
echo $path_parts['basename'], "\n"; // 'lib.inc.php'
echo $path_parts['extension'], "\n"; // 'php'
echo $path_parts['filename'], "\n"; // 'lib.inc'
?>

```