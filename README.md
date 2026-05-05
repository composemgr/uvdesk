## 👋 Welcome to uvdesk 🚀

Open-source helpdesk and support ticket system

## 📋 Description

Open-source helpdesk and support ticket system

## 🚀 Services

- **app**: nuttcorp/uvdesk:latest

### Infrastructure Components

- **db**: Mysql database


## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/uvdesk/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/uvdesk" ~/.local/srv/docker/uvdesk
cd ~/.local/srv/docker/uvdesk
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install uvdesk
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
DB_USER_NAME=uvdesk
DB_USER_PASS=changeme_db_password
DB_ADMIN_PASS=changeme_admin_password
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:59338

## 📂 Volumes

- `./volumes/data/db/mysql` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
