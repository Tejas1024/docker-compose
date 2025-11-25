# 4_docker_compose_examples.md

# 🧑‍💻 Docker Compose Examples

---

## Basic Compose YAML (Single Container)

version: "3.8"
services:
web:
image: nginx
ports:
- "8080:80"

text
- **web** runs Nginx and maps port 8080 (host) to 80 (container).

---

## Compose YAML with Volumes and Networks (Two Containers)

version: "3.8"
services:
web:
image: nginx
ports:
- "8080:80"
networks:
- appnet

db:
image: mysql:5.7
environment:
MYSQL_ROOT_PASSWORD: root
MYSQL_DATABASE: mydb
volumes:
- db-data:/var/lib/mysql
networks:
- appnet

volumes:
db-data:

networks:
appnet:
driver: bridge

text
- **web** = nginx frontend
- **db** = MySQL backend; stores data even after container deletion.

---

## Compose YAML with Named Containers, Volume, Network

version: '3'
services:
nginx-container:
image: nginx
container_name: nginx-container
volumes:
- vol1:/demo
networks:
- my-network
ports:
- "120:80"

volumes:
vol1:

networks:
my-network:
driver: bridge

text
- **nginx-container** is the web server with persistent data.
- **vol1** is the named Docker volume.
- **my-network** is the network for inter-container communication.