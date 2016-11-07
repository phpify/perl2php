# Functions

perl                | php
--------------------|---------------------
sub foo {<br> my @args = @_;<br>}                   | function foo() {<br>   $args = func_get_args(); <br>}
 
 
sub foo {
 $x = 5;
}




foo2( \@a, \%h );









php

function foo() {
 global $x;
 $x = 5;
}
 
function foo2($x, $y) {
}
 
foo2( $a, $h );