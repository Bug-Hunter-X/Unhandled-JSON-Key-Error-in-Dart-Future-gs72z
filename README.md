# Unhandled JSON Key Error in Dart Future

This repository demonstrates a common error in Dart when handling asynchronous operations and JSON responses. The code attempts to access a key that might not exist in the JSON data, leading to an exception that isn't always properly handled.

## The Problem
The `fetchData` function fetches data from an API.  If the API returns a JSON response missing a key the code attempts to access, a runtime exception occurs.

## The Solution
The improved solution includes a check to ensure the key exists before accessing it. This prevents the runtime error and handles the missing key gracefully.