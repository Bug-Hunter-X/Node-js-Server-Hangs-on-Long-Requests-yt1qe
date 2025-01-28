# Node.js Server Hang Issue

This repository demonstrates a common issue in Node.js where a long-running operation in a request handler can block the event loop, causing the server to become unresponsive to new requests. The `server.js` file contains the buggy code.  The solution is provided in `server-solution.js`.

**Problem:** The server freezes for 5 seconds while processing a request, making it unable to handle other requests during this time.

**Solution:** Using asynchronous operations or worker threads prevents blocking the main event loop.