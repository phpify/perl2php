# Functions

perl                | php
--------------------|---------------------
`sub foo { my @args = @_;}`                   | `function foo() {   $args = func_get_args(); }` 
`sub foo { $x = 5;}`                          | `function foo() { global $x; $x = 5;}`
`sub foo2( \@a, \%h );`                       | `function foo2($x, $y) {}`
`foo2( \@a, \%h );`                           | `foo2( $a, $h );`