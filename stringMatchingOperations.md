# String Matching Operations

perl                | php
--------------------|---------------------
`$s =~ m/(\w+)/;`                 | `preg_match( "/(\w+)/", $s, $match );`
`$substr = $1;`                   | `$substr = $match[1];`
`@all = ($s =~ m/(\w+)/g);`       | `preg_match_all( "/(\w+)/", $s, $match );<br>$all = $match[0];`
`$s =~ s/\s+/X/;`                 | `$s = preg_replace( "/\s+/", 'X', $s, 1 );`
`$s =~ s/\s+/X/g;`                | `$s = preg_replace( "/\s+/", 'X', $s );`
`$s =~ s/^\s+|\s+$//g;`           | `$s = trim($s);`
