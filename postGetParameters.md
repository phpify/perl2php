# POST / GET Parameters

perl                | php
--------------------|---------------------
\#form/hyperlink parameters:<br>\# s : single-valued<br>\# m : multi-valued<br><br> use CGI (:standard); | \#form/hyperlink parameters:<br>\# s   : single-valued<br>\# m[] : multi-valued<br>\#       (such as multi-selections<br>\#        and checkbox groups)<br>$PARAM<br>  = array_merge($_GET, $_POST);
$s = param('s');        | $s = $PARAM['s'];  # a scalar
@m = param('m');        | $m = $PARAM['m'];  # an array
@param_names = param(); | $param_names = array_keys($PARAM);
$num_params = param();  | $num_params = count($PARAM);






 


 

