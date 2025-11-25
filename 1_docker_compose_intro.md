# 1_docker_compose_intro.md

# 🐳 Docker Compose — Introduction

---

## 💡 What is Docker Compose?

Docker Compose is a tool to **define, run, and manage multi-container Docker applications**.  
All containers, networks, and volumes are described in a single file (`docker-compose.yml`), which you can run with one command:
docker compose up

 

---

## ✅ Purpose

Simplifies managing several containers (frontend, backend, database, etc.) that need to work together  
Easy to define interactions (networks, shared volumes) all in one place.

---

## 📄 What is a YAML File?

- Human-readable configuration format (uses indentation and key:value pairs)
- Used to configure services/apps (Docker Compose, Kubernetes, Ansible, etc.)
- Replaces brackets/tags with whitespace for structure

---

## 🧱 Docker Compose YAML File Structure

Sections:
- `services:` (lists containers)
- `networks:` (defines communication)
- `volumes:` (defines persistent storage)

Example:
services:
web:
image: nginx
networks:
- appnet
volumes:
- web-data:/usr/share/nginx/html

networks:
appnet:

volumes:
web-data:

 

---

## 📝 Key Points

- All the configuration lives in the YAML file
- `docker compose up` starts everything as defined