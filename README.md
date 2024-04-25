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

docker-compose up -d

docker-compose exec backend 
 Run the following command to install the dependencies:
```bash
composer install
php artisan key:generate
php artisan migrate
php artisan db:seed
```
