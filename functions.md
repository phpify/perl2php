# Functions

perl                | php
--------------------|---------------------
sub foo {<br> my @args = @_;<br>}                   | function foo() {<br>   $args = func_get_args(); <br>} 
sub foo {<br> $x = 5;<br>}                          | function foo() {<br> global $x;<br> $x = 5;<br>}
                                                    | function foo2($x, $y) {<br>}
foo2( \@a, \%h );                                   | foo2( $a, $h );