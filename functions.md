# Functions

perl                | php
--------------------|---------------------
sub foo {\n my @args = @_;\n}                   | function foo() {\n   $args = func_get_args(); \n}
 
 
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