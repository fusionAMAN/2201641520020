# 2201641520020

## Folder Structure

- **Backend/**
  - `server.js` → Core backend application implementing URL shortener functionality with expiry and statistics.  
  - `package.json`,  

- **Logging-Middleware/**
  - `server.js` → Express.js server with custom logging middleware that records request details.  
  - `package.json`,  




# 📌 Logging Middleware Service

This project implements a reusable **logging middleware** that sends structured logs to the **Evaluation Service API**.  
It demonstrates authentication, token management, and making authenticated API calls to log application events.

---


## Authentication
<img width="1768" height="912" alt="Screenshot 2025-09-08 134746" src="https://github.com/user-attachments/assets/b87dcc1d-7be4-41de-963e-c655b0f2bec0" />
<img width="1730" height="845" alt="image" src="https://github.com/user-attachments/assets/d6172d8b-bc08-4083-a813-ee8476458daf" />





## Running the Project
### Install dependencies
npm install express axios

## Start the server
node server.js

## Visit
GET http://localhost:3000/ 

<img width="1377" height="812" alt="Screenshot 2025-09-08 142949" src="https://github.com/user-attachments/assets/411011a4-543f-4e77-8eda-77c411d9f3a9" />



# Backend (URL-Shortner)
---

## 🚀 Features
- Create short URLs with optional custom shortcode.
- Each short URL has an *expiry time* (default: 30 minutes).
- Redirect from short URL to original URL.
- Track clicks with timestamp, referrer, and IP address.
- Fetch statistics for each shortcode.
---
## Technologies Used
- **Node.js**: Backend runtime environment.  
- **Express.js**: Web framework for building APIs and middleware.  
- **Moment.js**: Date/time handling for URL expiry.  
- **Nanoid**: Unique short code generation.  
---

## 📝 API Endpoints
### 1️⃣ Create a short URL
# http://localhost:3000/shorturls
{
  "url": "https://example.com/very-long-page",
  "validity": 10,
  "shortcode": "abc123"
}

![WhatsApp Image 2025-09-08 at 14 29 23_d2ea602e](https://github.com/user-attachments/assets/c09d6452-2762-4fd8-8892-f3da816cc905)

## Geeting UrL back. 
## http://localhost:3000/shorturls/abc123

![WhatsApp Image 2025-09-08 at 15 01 08_d7daa716](https://github.com/user-attachments/assets/0afe4408-b3f8-4fac-957b-2a99649d10d0)
