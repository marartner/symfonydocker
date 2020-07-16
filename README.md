# Symfony 5 docker containers

A Proof-of-concept of a running Symfony 5 application inside containers 
based on https://gitlab.com/martinpham/symfony-5-docker/-/tree/master/docker/database

```
git clone git@github.com:marartner/symfonydocker.git

cd symfonydocker

docker-compose up
```

## Compose

### Database (Mysql)

...

### PHP (PHP-FPM)

Composer is included

```
docker-compose run php-fpm composer 
```

Migrations are automatically run on `docker-compose up`

To run fixtures

```
docker-compose run php-fpm bin/console doctrine:fixtures:load
```

### Webserver (Nginx)

...
