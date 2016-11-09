# HTML Elements

perl                | php
--------------------|---------------------
use CGI (:standard);                                        | \# no need for that. 
$ref = "x.cgi";<br>a({href=>$ref}, "yy")                    | $ref = "x.php";<br>\<a href="\<?php echo $ref?\>"\>yy\</a\>
textfield({name=>"yy", size=>5})                            | <input type=text name=yy size=5>
password({name=>"yy", size=>5})                             | <input type=password name=yy size=5>
textarea({name=>"yy", cols=>5, rows=>2})                    | <textarea name=yy cols=5 rows=2></textarea>
submit({value=>"yy"})                                       | <input type="submit" value=yy>
button( {name=>"xx", value=>"yy", onclick=>"submit()" } )   | <input type="button" name="xx" value="yy" onclick="submit()"> 
%labels = (0=>'a',1=>'q',2=>'x');<br>popup_menu( { name=>"xx", values=\>[0..2], labels=\>\\%labels, size=\>4 } )     | \<select name="xx" size="4"\><br>\<?php<br>$labels = array(0=\>'a',1=\>'q',2=\>'x');<br>foreach (range(0,2) as $_)<br>  echo "\<option value='$_'\>",<br>       $labels[$_];<br>?\><br>\</select\>
@a = ('xx','yy','zz');<br>radio_group( { name=\>'nn', values=\> \\@a, default=\>'_',linebreak=\>1 } )                | $a = array('xx','yy','zz');<br>foreach ($a as $_)<br>  echo "\<input type=radio name=nn value='$_'\>$_\<br\>";
%labels = ('xx'=\>'L1','yy'=\>'L2');<br>@a = keys( %labels );<br>checkbox_group( { name=>'nn', values=> \\@a, labels=> \\%labels } )    | $labels = array('xx'=\>'L1','yy'=\>'L2');<br>foreach (array_keys($labels) as $_)<br>  echo "\<input type=checkbox name=nn value='$_'\>", $labels[$_];   
table( Tr( [ td(['a','b']), td(['x','y']) ] ) )            | \<table\><br>    \<tr\>\<td\>a\</td\>\<td\>b\</td\>\</tr\><br>    \<tr\>\<td\>x\</td\>\<td\>y\</td\>\</tr\><br>\</table\>

