# Environment

perl                | php
--------------------|---------------------
`%ENV`                | `$_SERVER` Server and execution environment information
`$ENV{REQUEST_METHOD}`| `$_SERVER[REQUEST_METHOD]` request method was used to access the page; e.g. 'GET', 'HEAD', 'POST', 'PUT'.
`$ARGV[$i]`           | `$argv[$i+1]` Array of arguments passed to script
`$0`                  | `$argv[0]  # Php/CGI only`
