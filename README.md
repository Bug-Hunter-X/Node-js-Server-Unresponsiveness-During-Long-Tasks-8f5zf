# Node.js Server Unresponsiveness During Long Tasks

This repository demonstrates a common issue in Node.js applications where long-running tasks can cause the server to become unresponsive.  The `server.js` file contains a simple HTTP server that simulates a long-running task.  This task blocks the event loop, preventing the server from handling new requests.

The solution, provided in `serverSolution.js`, uses asynchronous operations and a worker thread to avoid blocking the main event loop.