# 🐳 WordPress with MariaDB and phpMyAdmin using Docker

A complete WordPress development environment with MariaDB and phpMyAdmin, containerized with Docker Compose for easy setup and deployment.

## 🌟 Features

- Latest WordPress version
- MariaDB 10.5 database
- phpMyAdmin for database management
- Persistent database storage
- Custom PHP configuration
- Isolated development environment

## 🚀 Prerequisites

- Docker installed
- Docker Compose installed
- Ports 8080 and 8081 available

## 🛠️ Installation

1. Clone this repository:
   ```bash
   git clone [your-repository-url]
   cd docker-wordpress
   ```

2. Start the containers:
   ```bash
   docker-compose up -d
   ```

## 🌐 Access

- **WordPress**: http://localhost:8080
- **phpMyAdmin**: http://localhost:8081

## 🔧 Configuration

### Environment Variables

You can customize the following environment variables in the `docker-compose.yml` file:

- Database:
  - `MYSQL_DATABASE`: WordPress database name (default: `wordpress`)
  - `MYSQL_USER`: Database user (default: `user`)
  - `MYSQL_PASSWORD`: Database password (default: `password`)
  - `MYSQL_ROOT_PASSWORD`: Root password (default: `rootpassword`)

### PHP Configuration

Custom PHP settings can be modified in the `php-custom.ini` file.

## 📂 Directory Structure

- `./wordpress/`: WordPress installation files
- `./php-custom.ini`: Custom PHP configuration
- `docker-compose.yml`: Docker Compose configuration

## 🔄 Maintenance

### Stop the containers
```bash
docker-compose down
```

### Stop and remove all data
```bash
docker-compose down -v
```

### Update containers
```bash
docker-compose pull
docker-compose up -d
```

## 🔒 Security Notes

⚠️ **Important**: This setup uses default credentials for demonstration purposes. For production, please:
- Change all default passwords
- Use environment variables for sensitive data
- Consider using Docker secrets for production

## 🤝 Contributing

Feel free to submit issues and enhancement requests.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
