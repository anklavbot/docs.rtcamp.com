## Rename rtMedia Upload Directory

Add the following code in your theme's *functions.php* file to rename the **rtMedia** upload directory.

```php
function rename_rtmedia_upload_folder_name( $folder_name ) {
$folder_name = 'YourMedia';
return $folder_name;
}
add_filter( 'rtmedia_upload_folder_name', 'rename_rtmedia_upload_folder_name', 99, 1 );
```
