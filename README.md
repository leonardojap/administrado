# Nombre del Proyecto

Descripción breve del proyecto.

## Requisitos

- Docker
- Docker Compose

## Pasos para levantar el proyecto

1. Clona el repositorio:

```bash
git clone <url del repositorio>
cd <nombre del directorio del proyecto>
```
2. add you env file
3. Run the following command to build the containers and start the services:
```bash
docker-compose build

docker-compose up -d

docker-compose exec backend sh
```
4. Run the following command to install the dependencies:
```bash
composer install
php artisan key:generate
php artisan migrate
php artisan db:seed
```

