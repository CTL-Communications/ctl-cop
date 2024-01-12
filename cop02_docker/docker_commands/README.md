# Basic commands

## Important!

Locate the `docker-compose.yml` file in the repository and run commands from that directory.

## Local development common commands

```bash
# Build all services configured in the docker-compose.yml file
docker-compose build

# Run all services/containers in the background
docker-compose up -d

# Shutdown the application
docker-compose down

# Destroy - Shutdown and destroy all images and volumes associated with our app.
docker-compose down --rmi all --volumes

# View the status of our running services
docker-compose ps

# Connect to our application (SSH/login into our application’s shell)
docker exec -it ai8-ubuntu-1 bash 

# Connect to our database (Access our mysql database to run SQL queries)
docker exec -it ai8-mysql-1 mysql -uroot -psecret

# Inspect a container configuration (IP, network, volumes, etc)
docker inspect ai8-ubuntu-1 

# View a log report of all services within our app
docker-compose logs
```
