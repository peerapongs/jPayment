
README.TXT
==========

This PHP example code is written to show how transactions can be implemented 
using the Virtual Payment Client. 

The example HTML files can be simply installed into any directory of the Web
Server's ROOT directory. 

The xxx.php files must be saved in the appropriate directory that services 
php scripts. The .php file that will service the HTTP request is specified in 
the '<form action="/xxx.php" method="post">' parameter of the input HTML file. 
 
This 'ACTION' value may have to be changed for your installation.

The initial HTML page passes control to the php script when the submit button 
on the HTML page is clicked.

The MerchantID and Merchant Access Code is that value given to you by your 
Payment Provider.

In 3-Party Mode the example talks about a 'secure-hash-secret' found in both the 
DO.php and DR.php files. This is an optional security measure to detect if 
customers interfere with the data while in transit through their browser. It is 
not used for 2-Party transactions as the 2Party.php file communicates directly 
to the Virtual Payment Client and not through the customer's browser.

In 2-party mode the correct PHP 'CURL' library need to be installed on the 
machine servicing the 2Party.php file. There are different options here that may 
need to be commented/uncommented to work on your machine. This example is 
shipped with proxy enabled and a temporary SSL certificate disabled. 

author Dialect Solutions Group 2004
