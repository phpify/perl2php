# Data Structures

perl                | php
--------------------|---------------------

perl

%h = ('a'=>13, 'b'=>25);
@x = ('hi', 'there', 'all',);
 
@mix = ( \%h, \@x,
         [33..39],
	 { x=>15, yy=>23, },
       );
 
$mix[0]->{'b'}  # == 25
$mix[0]{'b'}    # == 25
$mix[2]->[2]    # == 35
$mix[2][2]      # == 35






php

$h = array('a'=>13, 'b'=>25);
$x = array('hi', 'there', 'all',);
 
$mix = array($h, $x,
	     range(33,39),
	     array('x'=>15, 'yy'=>23),
	    );
 
$mix[0]['b']  # == 25
 
$mix[2][2]    # == 35