## What is NPM?
- NPM is a package manager for Node.js packages, or modules if you like.
- www.npmjs.com hosts thousands of free packages to download and use.
- The NPM program is installed on your computer when you install Node.js

## What is a Package?
- A package in Node.js contains all the files you need for a module.
- Modules are JavaScript libraries you can include in your project.

## Download a Package
- Downloading a package is very easy.
- Open the command line interface and tell NPM to download the package you want.
- I want to download a package called "axios": </br>
` C:\Users\dbt>npm i axios `

## npm-init
create a package.json file
![npm-init images](https://github.com/darshan-trivedi-10/Image/blob/main/node-img/Screenshot%20(676).png)
[https://nodejs.org/api/packages.html](https://nodejs.org/api/packages.html)

## Stream 
- streams is process(read and write) data piece(chunks) without completing the
whole read or write operation, and therefore without keeping all the data in 
memory.
- There are four types of streams- readable streams, writable streams, duplex
and transform streams.

Ex :- input.txt will contain a lot of text and paragraphs.
```js
const fs = require('fs');
const transformStream = require('stream');
let fileStream = fs.createReadStream(__dirname + "/input.txt");
let outputStream = process.stdout;
// readstream.pipe(writestream)
let middleStream = new transformStream.Transform({
    transform(chunk, enc, nextCB) {
        let modifiedChunk = chunk.toString().toUpperCase();
        this.push(modifiedChunk);
        setTimeout(nextCB, 1000);
        // nextCB();
    }
});
// fileStream.pipe(outputStream);
let newReadableStream = fileStream.pipe(middleStream);
newReadableStream.pipe(outputStream);

```
[https://nodejs.org/api/stream.html](https://nodejs.org/api/stream.html)
