# 🎬 Movie Recommendation Backend  

A backend service for a movie recommendation application, built with **Django**. This project integrates with **The Movie Database (TMDb) API** to fetch trending and recommended movies, supports **user authentication**, allows users to save their favorite movies, and implements **caching** for high performance.  

---

## 📌 Overview  

This backend mirrors real-world backend development scenarios where performance, security, and user-centric design are crucial. It provides APIs for:  

- 🔑 **User Authentication** (JWT-based).  
- 🎥 **Movie Data Retrieval** from TMDb API.  
- ⭐ **User Preferences** (saving/retrieving favorite movies).  
- ⚡ **Performance Optimization** via Redis caching.  
- 📖 **Comprehensive API Documentation** with Swagger.  

---

## 🎯 Project Goals  

1. **API Creation**  
   - Fetch trending and recommended movies.  
   - Robust error handling for external API calls.  

2. **User Management**  
   - Secure authentication with JWT.  
   - Save and retrieve favorite movies.  

3. **Performance Optimization**  
   - Use Redis to cache trending/recommended movie data.  
   - Reduce external API call frequency and improve response times.  

4. **Documentation**  
   - Swagger-powered API docs at `/api/docs`.  

---

## 🛠️ Technologies Used  

- **Django** → Backend framework.  
- **PostgreSQL** → Relational database.  
- **Redis** → Caching system for performance.  
- **TMDb API** → Third-party movie database.  
- **Swagger** → API documentation.  
- **djangorestframework-simplejwt** → JWT authentication.  

---

## 📂 Project Structure  

```bash
Movie-Recommendation/
│── manage.py
│── movie_recommendation/       # Main project settings
│   ├── settings.py
│   ├── urls.py
│── movies/                     # Movies app (TMDb integration, caching)
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│── users/                      # Users app (authentication, favorites)
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│── requirements.txt
│── README.md
