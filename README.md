# Installation
Clone or download the repo

- `cd {download_dir}`
- `cp .env.example .env` 
- `docker-compose build`
- `mkdir symfony`
- `cd symfony`  
- `download or copy symfony`, visit [Symfonys setup guide](https://symfony.com/doc/current/setup.html) for installation options

After symfony installation start the container
- `docker-compose build` to build all container
- `docker-compose up -d` to start in detached mode
- `docker-compose exec symfony /bin/bash` to connect to the symfony container
- `composer install && composer update`

Done