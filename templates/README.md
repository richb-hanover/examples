# templates

Display a page with a template filled in from a JSON object in the program. To invoke, the following command begins listening on localhost:3000.

    node --harmony index.js

To see results:

    http://localhost:3000
    

## Interesting points

1. The `render` variable is set to a view built from an Embedded Javascript (.ejs) file in the views directory.
2. The app.use() function yields to the render() function, which substitutes data from the `user` JSON object.
3. render() returns its result to this.body, which is then sent to the web client.