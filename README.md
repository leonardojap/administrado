# Courses test 

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
2. Agrega tu archivo .env en la carpeta raiz de laravel, mirar el ejemplo en .env.example
3. Corre el siguiente comando para construir y correr el proyecto con docker:
```bash
docker-compose build

docker-compose up -d

docker-compose exec backend sh
```
4. Una vez ejecurtado el ultimo comando, ejecutar los siguientes comandos en la misma consola:
```bash
composer install
php artisan key:generate
php artisan migrate
php artisan db:seed
```

