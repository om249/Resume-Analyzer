# Resume Analyzer

## Project Overview

Resume Analyzer is a full-stack web application that uses Google Gemini AI to analyze resumes. It extracts key skills, calculates an ATS score, provides personalized improvement suggestions, and recommends relevant job opportunities. The application also includes secure authentication with email verification, password reset, and JWT-based authorization.

---

## Technology Stack

### Frontend
- React.js
- HTML5
- CSS3
- JavaScript
- Vite

### Backend
- Java
- Spring Boot
- Spring Security
- JWT Authentication
- Maven

### Database
- MySQL

### APIs & Services
- Google Gemini API
- Brevo API
- Adzuna API
- Apache Tika

---

## Features

- User Registration & Login
- Email Verification
- Forgot Password
- Resume Upload (PDF)
- AI-Based Resume Analysis
- ATS Score & Feedback
- Skill Extraction
- Job Recommendations
- Secure JWT Authentication 

---

## Preview

<p align="center">
  <img width="30%" src="https://github.com/user-attachments/assets/df7bb0c1-1f10-478d-b8c9-c2b1bf2369f4" />
  <img width="30%" src="https://github.com/user-attachments/assets/1c65a0cc-c915-4103-a7fe-30a975639ab0" />
  <img width="30%" src="https://github.com/user-attachments/assets/b8ca21ad-7c2f-470d-ad5d-73119b8fd9f1" />
</p>

<p align="center">
  <img width="30%" src="https://github.com/user-attachments/assets/3f945bf1-84dd-4052-9c65-709f512ae0a4" />
  <img width="30%" src="https://github.com/user-attachments/assets/d04af8b7-4e12-4948-94c6-3b1f15340180" />
  <img width="30%" src="https://github.com/user-attachments/assets/a0c6f513-2108-41c8-98b5-91e86d27d398" />
</p>


## Setup Instructions

1. Clone the repository.
2. Configure the MySQL database.
3. Update the required environment variables in `application.properties`.
4. Run the Spring Boot application.
5. Open the application in your browser.

```
http://localhost:8080
```

---

## Database Configuration

```properties
spring.datasource.url=YOUR_DATABASE_URL
spring.datasource.username=YOUR_DATABASE_USERNAME
spring.datasource.password=YOUR_DATABASE_PASSWORD

spring.jpa.hibernate.ddl-auto=update
```

Required API Keys:

- Google Gemini API
- Brevo API
- Google OAuth Client ID & Secret
- Adzuna API
- JWT Secret Key

---

## API Endpoints

### Authentication

| Method | Endpoint |
|--------|----------|
| POST | `/resumeAnalyser/entry/v1/register` |
| POST | `/resumeAnalyser/entry/v1/login` |
| POST | `/resumeAnalyser/entry/v1/verifyEmail` |
| POST | `/resumeAnalyser/entry/v1/resetOtpSent` |
| POST | `/resumeAnalyser/entry/v1/verifyResetOtp` |
| POST | `/resumeAnalyser/entry/v1/resetPassword` |

### Resume

| Method | Endpoint |
|--------|----------|
| POST | `/resumeAnalyserCore/service/v1/extract` |
| GET | `/resumeAnalyserCore/service/v1/lastReport` |
| POST | `/resumeAnalyserCore/service/v1/logout` |
| POST | `/resumeAnalyserCore/service/v1/deleteAccount` |
| POST | `/resumeAnalyserCore/service/v1/isValid` |

---

## Application Screenshots

> Add screenshots of the following pages:

- Home Page
- Login Page
- Register Page
- Dashboard
- Resume Upload
- Resume Analysis Result
- Job Recommendations
