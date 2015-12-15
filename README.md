# wp-multiple-insert
a method for inserting multiple rows in a safer and faster way

# usage example
```
       $insert_arrays = array();
       foreach($assets as $asset) {
	   $time = current_time( 'mysql' );
       $insert_arrays[] = array(
       'type' => "multiple_row_insert",
       'status' => 1,
       'name'=>$asset,
       'added_date' => $time,
       'last_update' => $time);
     
       }
     
       wp_insert_rows($insert_arrays);
 ```
 
 
 source : http://stackoverflow.com/a/12374838/1194797