
# Sync and Async Web Server on Python

## Objective
Develop web servers in Python in 2 versions: a fisrt simple synchronous (sync) web server using only the `socket` module and second an asynchronous (async) web server using the `aiohttp` framework.

### Main Steps:
1. **Synchronous (Sync) Web Server:**
   - Create a simple synchronous web server using the `socket` module.
   - The sync server should listen on `localhost` at port `8000`.
   - Implement a single route `/hello` that responds with a plain text message "Hello, World!".
   - Demonstrate handling HTTP requests synchronously.

2. **Asynchronous (Async) Web Server:**
   - Create an asynchronous web server using the `aiohttp` framework.
   - The async server should listen on `localhost` at port `8000`.
   - Implement two routes:
     - Route 1: `/hello`
       - Respond with a plain text message "Hello, World!".
     - Route 2: `/echo`
       - Accept POST requests.
       - Respond with the JSON representation of the received POST data.
   - Use asynchronous programming features provided by `aiohttp`.
   - Demonstrate the use of asynchronous functions, `asyncio`, and the `aiohttp` library to handle requests concurrently.

### Additional Challenges (For bouth servers):
1. **Middleware:**
   - Implement a middleware that adds a custom header to every response.

2. **Error Handling:**
   - Implement error handling for common HTTP errors (e.g., 404 Not Found, 500 Internal Server Error).

3. **Unit Tests:**
   - Write unit tests for the main functionality of both the sync and async servers.

4. **Dockerization (Optional):**
   - Create a Dockerfile for each server to containerize both the sync and async applications.

### Submission:
- Submit the codebase along with a brief README explaining how to run both the sync and async servers and any additional features implemented.

### Note:
- Use Python 3.10 or above.
- Use poetry as dependency manager and config store if you need.
- Add popular linters and formattetes.
- Write code due PEP8.