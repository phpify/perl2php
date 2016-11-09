# Hashes

perl                | php
--------------------|---------------------
%h = ();                                    | $h = array();
%h = ( 'x' => 'y', 'z' => 'w' );            | $h = array( 'x' => 'y', 'z' => 'w' );
$h{'x'} = 7;                                | $h['x'] = 7;
while (($key,$value) = each(%h))<br>{ .. }  | foreach ($h as $key =\> $value)<br>{ .. }
$a = keys(%h);                              | $a = array_keys($h);
$b = values(%h);                            | $b = array_values($h);
delete $h{'x'};                             | unset( $h['x'] );
