# URL Shortener Project

## Summary

This project is a simple URL shortener service written in Go. It provides a basic web server that allows users to shorten URLs and then redirect to the original URL using the generated short link. The service is built using the `chi` router for handling HTTP requests and `shortuuid` for generating unique keys for the shortened URLs.Using this as a way to solidify my go knowledge.

### Key Features

- Shorten URLs via a simple HTTP POST request.
- Redirect to the original URL using the generated short link.
- In-memory storage of URL mappings.

### Endpoints

- `POST /shorten-url`: Accepts a URL and returns a shortened version.
- `GET /shorten-url/{key}`: Redirects to the original URL based on the provided key.

## To-Do List

1. **Error Handling and Logging**: Enhance error handling and provide more detailed logs.
2. **Data Persistence**: Implement a database for persistent storage of URL mappings.
3. **Concurrency Handling**: Optimize concurrent access to the URL mappings.
4. **Input Validation**: Add validation for input URLs.
5. **Custom Short URL Paths**: Allow users to specify custom paths for shortened URLs.
6. **Rate Limiting**: Implement rate limiting to prevent abuse of the service.
7. **Dockerization**: Containerize the application for easier deployment.
8. **Metrics and Monitoring**: Add system monitoring and performance metrics.
9. **Testing**: Add unit and integration tests.
10. **Configurable Base URL**: Make the base URL configurable.
11. **Graceful Shutdown**: Implement graceful shutdown for the server.
