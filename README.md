# OTP Authentication API with Redis

A backend OTP authentication API built with **Node.js, Express.js, and Redis**.  
The project demonstrates OTP generation, verification, automatic expiration using Redis TTL, and single-use OTPs.

Redis is run locally using **Docker Compose**, making the project easy to set up and run.

---

## 🚀 Features

- Generate a random 6-digit OTP
- Store OTPs securely in Redis
- Automatic OTP expiration using Redis TTL
- Verify OTPs
- Prevent OTP reuse after successful verification
- Check the remaining TTL of an OTP
- RESTful API endpoints
- Redis containerized using Docker
- Easy local development setup

---

## 🛠️ Tech Stack

- **Node.js**
- **Express.js**
- **Redis**
- **ioredis**
- **Docker**
- **Docker Compose**
- **Postman** for API testing

---

## 📁 Project Structure

```text
otp-authentication-redis/
│
├── src/
│   └── index.js
│
├── docker-compose.yml
├── package.json
├── package-lock.json
├── .gitignore
└── README.md
```
---
🔐 Security Note

This project is intended as a demonstration of OTP authentication and Redis TTL.

For a production implementation, additional security measures should be considered, such as:

- Sending OTPs through an SMS/email provider
- Rate limiting OTP requests
- Limiting verification attempts
- Hashing OTPs before storage
- Preventing OTP enumeration
- Input validation
- HTTPS
- Secure logging practices
- Authentication and authorization controls
