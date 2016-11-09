# mySQL database access

perl                | php
--------------------|---------------------
use DBI;<br>$dbh = DBI->connect(<br>  'DBI:mysql:test:localhost',<br>  $usr,$pwd<br>);     | $dbh = mysql_connect(<br>  'localhost', $usr, $pwd<br>);<br>mysql_query('USE test')
$dbh->do( $sql_op )                                                                        | mysql_query( $sql_op );
$query = $dbh->prepare( $sql_op );<br>$query->execute();                                   | $results = mysql_query( $sql_op );
while(<br> @record = $query->fetchrow() )<br>{ .. }                                        | while($record = mysql_fetch_row($results))<br>{ .. }
$dbh->quote($val)                                                                          | "'" . addslashes($val) . "'"