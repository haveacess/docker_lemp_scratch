Faster creating project based on **LEMP** (Linux, NGINX, MYSQL, PHP) from scratch in Docker container. Laravel


## Using 

### Development
```text
# create symbolink
ln -s docker-compose.dev.yml docker-compose.yml

# create .env file
mv .env.dev.example .env
```

### Production
```text
# create symbolink
ln -s docker-compose.prod.yml docker-compose.yml

# create .env file
mv .env.prod.example .env
```

### For both environments (Optional)
```text
# rebuild containers except cache
docker compose build --no-cache

# Up containers with build option
docker compose up -d --build
```