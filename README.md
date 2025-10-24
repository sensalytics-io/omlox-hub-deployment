# 🚀 Sensalytics Omlox Hub – Quickstart Guide

## ✅ Prerequisites

- 🐳 Docker
- 📦 Docker Compose

## ⚙️ Setup Instructions

1. **Clone the repository.**
2. **Request a trial license** by emailing: `contact@sensalytics.io`
3. **Save the received `.slyc` license file** to the `license` folder.
4. **Edit `docker-compose.yml`:**  
   Replace `YOUR_LICENSE` with the actual filename of your `.slyc` license.
5. **Start the service:**

   ```bash
   docker-compose up -d
   ```
6. 🌐 Access the API or Swagger UI:
   - API: curl http://localhost/v2/zones
   - Swagger UI: http://localhost/swagger-ui/index.html