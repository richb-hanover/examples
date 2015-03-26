# upload

Upload a file to a temporary directory on the server. To invoke, the following command begins listening on localhost:3000.

    node --harmony index.js

To see results:

    http://localhost:3000
    then select a file to upload and click "Upload"

## Interesting points

1. The application serves out files from public/ as indicated in the first app.use() function
2. The next app.use() ignores any request that isn't a POST. 
3. If it is a POST, the function calls fs.createWriteStream() on a temporary directory, then uses pipe() to copy the data into the local file system file.
