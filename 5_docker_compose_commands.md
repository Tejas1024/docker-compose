# 5_docker_compose_commands.md

# 🧑‍💻 Docker Compose & Cleanup Commands

---

## Docker Compose Workflow

- Create YAML file (`docker-compose.yml`)
- Run all containers as described in YAML

## Common Commands

| Command                              | Description                                           |
|---------------------------------------|------------------------------------------------------|
| docker compose up                     | Create and start all containers/services              |
| docker compose up -d                  | Run containers in background ("detached" mode)        |
| docker compose ps                     | List running containers created by Compose            |
| docker compose exec <service> <cmd>   | Run command inside a running container (e.g. bash)    |
| docker compose stop                   | Stop running containers (but don’t remove)            |
| docker compose start                  | Start stopped containers                             |
| docker compose restart                | Restart (stop/start) containers                      |
| docker compose down                   | Stop and remove containers & networks                 |
| docker compose down -v                | Stop and remove containers, networks, and volumes     |
| docker compose build                  | Build/rebuild images specified in YAML                |
| docker compose -f PATH up             | Use compose file at different path                    |
| docker volume ls                      | List volumes                                          |
| docker volume prune -y                | Remove unused volumes                                 |
| docker network prune -y               | Remove unused networks                                |

**Note:**  
- `stop` = stops containers, doesn't delete  
- `down` = stops & deletes containers/networks  
- `down -v` = deletes containers/networks/volumes (⚠️ data lost)

---

## Example: Execute Command Inside Container

Open shell inside container named "web":
docker compose exec web bash

 

List files in "nginx-container":
docker compose exec nginx-container ls

 
