perl

%h = ();
 
%h = ( 'x' => 'y',
       'z' => 'w',
     );
 
$h{'x'} = 7;
 
while (($key,$value) = each(%h))
{ .. }
 
$a = keys(%h);
$b = values(%h);
 
delete $h{'x'};






php

$h = array();
 
$h = array( 'x' => 'y',
            'z' => 'w',
          );
 
$h['x'] = 7;
 
foreach ($h as $key => $value)
{ .. }
 
$a = array_keys($h);
$b = array_values($h);
 
unset( $h['x'] );