# stream-server-side-events

This program continually sends events to the web browser. It simulates a series of log file entries that have been appended to a file.

To invoke, the following command begins listening on localhost:3000.

    node --harmony app.js

To see results:

    http://localhost:3000
    
You will see a succession of lines containing "data:" with an increasing number. This will continue as long as you keep the browser window open.

## Interesting points

1.
