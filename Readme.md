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
