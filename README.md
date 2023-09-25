# NodeJS Multithreading

https://www.digitalocean.com/community/tutorials/how-to-use-multithreading-in-node-js

## To measure how long it takes to get the response from the `/blocking` route:


Open 2 terminals.

In your 1st terminal, run the `without-multithreading.js` or `single_worker/index.js` or `four_workers/index.js` file. It will start the server:

```sh
node without-multithreading.js
```
or
```sh
cd single_worker
node index.js
```
or
```sh
cd four_workers
node index.js
```

Next, go to your 2nd terminal and:

```sh
time curl --get http://localhost:3000/blocking
```
