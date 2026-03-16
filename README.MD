# URL Shortener API

A backend service built using **Java and Spring Boot** that converts long URLs into short, shareable links.  
When a user accesses the short link, the service redirects them to the original URL.

This project demonstrates backend development concepts such as **REST APIs, database design, URL mapping, and HTTP redirection**.

---

## 🚀 Features

- Generate short URLs from long URLs
- Redirect users to the original URL
- Store URL mappings in database
- Track number of clicks on each shortened URL
- RESTful API design

---

## 🛠 Tech Stack

- Java
- Spring Boot
- Spring Data JPA
- MySQL / H2 Database
- Maven
- REST APIs

---

## 📂 Project Structure


src
├── controller
│ URLController.java
├── service
│ URLService.java
├── repository
│ URLRepository.java
├── model
│ URL.java
└── UrlShortenerApplication.java


---

## 📌 API Endpoints

### Create Short URL

POST /shorten

Example Request


{
"url": "https://example.com
"
}


Example Response


{
"shortUrl": "http://localhost:8080/abc123
"
}


---

### Redirect to Original URL

GET /{shortCode}

Example


GET /abc123


The service redirects to the original URL.

---

### Get URL Analytics

GET /analytics/{shortCode}

Returns number of clicks and metadata.

---

## 🗄 Database Schema

URL_TABLE

id
original_url
short_code
click_count
created_at


---

## ▶️ How to Run the Project

1. Clone the repository


git clone https://github.com/yourusername/url-shortener-api.git


2. Navigate to project directory


cd url-shortener-api


3. Run the application


mvn spring-boot:run


4. Open in browser


http://localhost:8080


---

## 💡 Learning Outcomes

- Building REST APIs using Spring Boot
- Designing database schemas
- Implementing URL mapping systems
- Understanding HTTP redirects
- Basic backend system design

---

## 📈 Future Improvements

- Add user authentication
- Custom short URLs
- Expiration for URLs
- Rate limiting
- Redis caching

---

## 👨‍💻 Author

Pranav Ganorkar
