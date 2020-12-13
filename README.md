# Php-integration-wih-python
PHP and Python Integration

I have struggling for integrating python on php.
Solution is this.

Write this code snippet when you are using serval version of pyhon(including anaconda)


          import sys
          import os

          os.chdir("C:/Users/sos/AppData/Roaming/Python/Python39/site-packages/")
          sys.path.append("C:/Users/sos/AppData/Roaming/Python/Python39/site-packages/")


In the php code


            $argument = str_replace(" ",",,,", $query);
            $output = exec('"C:\Program Files\Python39\python" scrapper.py '. "$argument");
            
Thanks.
