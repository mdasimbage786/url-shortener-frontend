# 🔗 LinkShrink - URL Shortener

A modern, beautiful URL shortener with analytics built using Spring Boot and Vanilla JavaScript.

![LinkShrink](https://img.shields.io/badge/LinkShrink-URL%20Shortener-6366f1?style=flat-square)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)

## ✨ Features

- 🚀 Instant URL shortening
- 📊 Real-time click analytics
- 🎨 Modern glassmorphism UI
- 📱 Fully responsive design
- 🔍 Filter and search links
- 📋 One-click copy to clipboard

## 🛠️ Tech Stack

**Backend:** Spring Boot, Spring Data JPA, H2/PostgreSQL  
**Frontend:** HTML5, CSS3, Vanilla JavaScript

## 🚀 Quick Start

### Prerequisites
- Java 17+
- Maven 3.6+

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/linkshrink.git
cd linkshrink
```

2. **Run the backend**
```bash
mvn spring-boot:run
```
Backend runs on `http://localhost:8080`

3. **Open the frontend**
```bash
# Open index.html in browser or use a server
python -m http.server 8000
```

## 📡 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/url/create` | Create short URL |
| GET | `/api/url/all` | Get all URLs |
| GET | `/api/url/{shortCode}` | Redirect to original URL |
| DELETE | `/api/url/{shortCode}` | Delete URL |

### Example Request
```bash
curl -X POST http://localhost:8080/api/url/create \
  -H "Content-Type: application/json" \
  -d '{"originalUrl": "https://example.com/long-url"}'
```

## 📁 Project Structure

```
linkshrink/
├── src/main/java/          # Backend code
├── src/main/resources/     # Configuration & static files
├── index.html              # Frontend
└── pom.xml                 # Maven dependencies
```

## 🎨 Customization

Change colors in CSS:
```css
:root {
    --primary: #6366f1;
    --secondary: #8b5cf6;
}
```

## 🚢 Deployment

**Backend:** Deploy to Render, Railway, or Heroku  
**Frontend:** Deploy to Netlify, Vercel, or GitHub Pages

Update `API_BASE_URL` in JavaScript to your production URL.

## 📝 License

MIT License - feel free to use for personal or commercial projects.

## 👤 Author

**Mohammedasim Bage**  
GitHub: [@mdasimbage786](https://github.com/mdasimbage786)

## ⭐ Support

Give a ⭐️ if you like this project!

---

**Built with ❤️ using Spring Boot & Vanilla JS**
