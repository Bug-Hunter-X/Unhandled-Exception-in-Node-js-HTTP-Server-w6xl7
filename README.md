# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common error in Node.js: unhandled exceptions in HTTP servers.  The `server.js` file shows a server that throws an error without proper handling. The `serverSolution.js` file shows a corrected version.

## Problem

The original server throws an exception when a request is made to `/error`. Because this exception is unhandled, the entire server process crashes.  This is problematic for production applications.

## Solution

The improved server uses a `try...catch` block to handle the exception gracefully.  It logs the error to the console and sends a proper error response to the client.