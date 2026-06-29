# coco-bliss--Karikku-app-
Coco Bliss
A lightweight, single-page web application for a premium tropical coconut brand. Built with HTML5, CSS3, and Vanilla JavaScript, and containerized using a minimal Nginx Alpine image.

Architecture
This project uses a static architecture. The entire frontend—including DOM manipulation, scroll reveals, and WebAudio API integrations—is contained within a single file payload. It is served via Nginx, ensuring high throughput and minimal memory footprint.

Prerequisites

Docker installed on your host machine.

Local Development & Deployment

You do not need to build the image from scratch since it is hosted on DockerHub.

Pull the Image:
Fetch the pre-built image from the public registry:

Bash
docker pull diabolicalwillow/karikkuapp:v1
Run the Container:
Execute the container and map it to port 8080 on your local machine:

Bash
docker run -d -p 8080:80 --name coco-bliss diabolicalwillow/karikkuapp:v1
Access the Application:
Navigate to http://localhost:8080 in your browser.

Infrastructure Details

Base Image: nginx:alpine

Port Exposure: Exposes port 80 internally

Asset Location: Static files are served directly from /usr/share/nginx/html
