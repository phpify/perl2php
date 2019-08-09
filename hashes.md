# Hashes

perl                | php
--------------------|---------------------
`%h = ();`                                    | `$h = array();` emty array
`%h = ( 'x' => 'y', 'z' => 'w' );`            | `$h = array( 'x' => 'y', 'z' => 'w' );` array with key and value
`$h{'x'} = 7;`                                | `$h['x'] = 7;`
`while (($key,$value) = each(%h))<br>{ .. }`  | `foreach ($h as $key => $value){ .. }` get key and and value from array
`$a = keys(%h);`                              | `$a = array_keys($h);`  Return all the keys or a subset of the keys of an array
`$b = values(%h);`                            | `$b = array_values($h);` Return all the values of an array
`delete $h{'x'};`                             | `unset( $h['x'] );` Unset a given variable
