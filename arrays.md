# Arrays

[Introduction Arrays php](https://www.php.net/manual/en/intro.array.php)
[ Arrays ](https://www.php.net/manual/en/book.array.php)

 perl                      | php                        
-------------------------- | -------------------------- 
`@a = ();`                 | `$a = array();`                        
`@a = ( 'xx', 11, 33.5, );`| `$a = array( 'xx', 11, 33.5, );`        
`@a = 12..33;`             | `$a = range(12,33);` Create an array containing a range of elements
`$a[2] = 'something';`     | `$a[2] = 'something';`
`$len = scalar(@a);`       | `$len = count($a);` Count all elements in an array, or something in an object
`$len = @a;`               | `$len = count($a);`
`@a3 = ('xx', @a1, @a2);`  | `$a3 = array_merge('xx', $a1, $a2);`
`($x, $y) = @a;`           | `list($x, $y) = $a;`
`$a[@a] = 'new'; # push`   | `$a[] = 'new'; # push`
`push`                     | `array_push` Push one or more elements onto the end of array
`pop`                      | `array_pop` Pop the element off the end of array
`shift`                    | `array_shift` Shift an element off the beginning of array
`unshift`                  | `array_unshift` Prepend one or more elements to the beginning of an array
`splice`                   | `array_splice` Remove a portion of the array and replace it with something else
`foreach $i (@a) { .. }`   | `foreach ($a as $i) { .. }` The foreach construct provides an easy way to iterate over arrays. foreach works only on arrays and objects, and will issue an error when you try to use it on a variable with a different data type or an uninitialized variable. There are two syntaxes:
`@a = split( '\|', $s );`  | `$a = preg_split( '/\|/', $s, -1, PREG_SPLIT_NO_EMPTY );`  Split string by a regular expression
`@a = split( '\s+', $s );` | `$a = preg_split( '/\s+/', $s, -1, PREG_SPLIT_NO_EMPTY );`
`$s = join( '|', @a );`    | `$s = join( '|', $a );`