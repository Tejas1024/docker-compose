# 6_assignment_static_site.md

# 📝 Assignment: Host a Static Website with Docker Compose

---

## Task

Host a static website using Docker Compose and Nginx.

---

## Folder Structure

myproject/
website/
index.html
docker-compose.yml

 

- `website`: contains your static web files (HTML, CSS, etc.)
- `docker-compose.yml`: configuration file

---

## docker-compose.yml Example

version: "3"
services:
web:
image: nginx
container_name: static-website
ports:
- "8080:80"
volumes:
- ./website:/usr/share/nginx/html

 

- `ports` maps local port 8080 to Nginx port 80
- `volumes` mounts local "website" folder to Nginx's HTML directory

---

## Commands to Run

Inside `myproject/`:

docker compose up -d

 

Open browser at:
http://localhost:8080

 
Your static site is now live.

---

## Stop and Clean-Up

To stop and remove everything (including volumes):

docker compose down -v

 