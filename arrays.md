# Arrays


 perl                      | php                        
-------------------------- | -------------------------- 
@a = ();                   | $a = array();                        
@a = ( 'xx', 11, 33.5, );  | $a = array( 'xx', 11, 33.5, );        
@a = 12..33;               | $a = range(12,33);
$a[2] = 'something';       | $a[2] = 'something';
$len = scalar(@a);         | $len = count($a);
# or                       | 
$len = @a;                 | $len = count($a);
@a3 = ('xx', @a1, @a2);    | $a3 = array_merge('xx', $a1, $a2);
($x, $y) = @a;             | list($x, $y) = $a;
$a[@a] = 'new'; # push     | $a[] = 'new'; # push
push                       | array_push
pop                        | array_pop
shift                      | array_shift
unshift                    | array_unshift
splice                     | array_splice
foreach $i (@a) { .. }     | foreach ($a as $i) { .. }
@a = split( '\|', $s );    | $a = preg_split( '/\|/', $s, -1, PREG_SPLIT_NO_EMPTY );
@a = split( '\s+', $s );   | $a = preg_split( '/\s+/', $s, -1, PREG_SPLIT_NO_EMPTY );
$s = join( '|', @a );      | $s = join( '|', $a );