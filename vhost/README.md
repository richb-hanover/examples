# vhost

Respond to virtual host queries: example.com and www.example.com have different response from bar.example.com. 

To invoke, set up `/etc/hosts` to return localhost for all three domain names, then enter the following command to begin listening on localhost:3000.

    node --harmony app.js

To see results:

    http://example.com:3000
    http://www.example.com:3000
    http://bar.example.com:3000    

## Interesting points

1. 
