# Flask on Docker

## Overview

This repository contains a simple Flask web service running on Docker, using Postgres, Gunicorn, and Nginx. The project follows the tutorial from TestDriven.io and allows users to upload and view images and other media files.

Below is an animated GIF showing the image upload process:

![ezgif-8420e452f9f16a](https://github.com/user-attachments/assets/2c10eda0-f363-4808-a488-4918b5769856)

## Build Instructions

### Prerequisites

- Docker
- Docker Compose
- Git

### Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/lucasLang0/flask-on-docker.git
   cd flask-on-docker
   ```

2. Create a `.env.prod.db` file (not included in the repository)

3. Build and start the services:

   ```bash
   docker compose up --build
   ```

4. Open your browser and navigate to:

   ```
   http://localhost:5454
   ```

5. To stop the services:

   ```bash
   docker compose down
   ```

## Notes

- Ensure that `.env.prod.db` is **never committed to GitHub** to prevent exposing sensitive credentials.
- If using this project in production, consider additional security measures like SSL certificates and stricter database configurations.
