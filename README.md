# Linkly - URL Shortener Backend Service

## Overview
Linkly is a backend URL shortening service built using Spring Boot. It provides secure JWT-based authentication, URL shortening, URL redirection, click tracking, and analytics through RESTful APIs.

## Features
- User Registration
- User Login
- JWT Authentication
- URL Shortening
- URL Redirection
- Click Analytics
- User-specific URL Management

## Tech Stack
- Java 21
- Spring Boot
- Spring Security
- JWT
- Spring Data JPA
- MySQL
- Maven
- Lombok

## Architecture

Controller
↓
Service
↓
Repository
↓
MySQL

## API Endpoints

### Authentication
POST /api/auth/public/register
POST /api/auth/public/login

### URL Management
POST /api/urls/shorten
GET /api/urls/myurls

### Analytics
GET /api/urls/analytics/{shortUrl}
GET /api/urls/totalClicks

### Redirect
GET /{shortUrl}

## Future Enhancements
- Redis Caching
- Docker Support
- URL Expiration
- Custom Aliases
- Swagger Documentation