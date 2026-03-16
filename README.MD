# URL Shortener API

A backend application built using **Spring Boot** that converts long URLs into short and shareable links.  
When a user accesses the shortened URL, the service redirects them to the original URL.

This project demonstrates concepts such as **REST API development, URL mapping, database storage, and HTTP redirection.**

---

## Tech Stack

- Java
- Spring Boot
- Spring Data JPA
- H2 Database
- Maven
- REST APIs
- JUnit

---

## Features

- Generate short URLs from long URLs
- Redirect users to the original URL
- Store URL mappings in database
- Simple REST API architecture
- Lightweight in-memory database for development

---

## API Endpoints

### Create Short URL

POST /shorten?url={fullURL}

Example

POST /shorten?url=https://example.com

Response

{
  "shortenedURL": "abc123",
  "fullURL": "https://example.com",
  "createdAt": "2026-03-16"
}

---

### Redirect to Original URL

GET /{shortCode}

Example

GET /abc123

The service redirects to the stored original URL.

---

## How to Run

Clone the repository

git clone https://github.com/yourusername/url-shortener-api.git

Navigate to project directory

cd url-shortener-api

Run the application

mvn spring-boot:run

Server runs on

http://localhost:8080

---

## Future Improvements

- Custom short URLs
- Click analytics
- User authentication
- URL expiration
- Redis caching

---

## Author

Pranav Ganorkar
