# Contactbook

![user accounts](https://user-images.githubusercontent.com/4499581/78510090-af644e00-778a-11ea-89fa-0bb3aadb2587.png)
![contactbook](https://user-images.githubusercontent.com/4499581/78510091-b12e1180-778a-11ea-8e37-2f51686820fb.png)

## Install

clone the repo and run `composer install` then `symfony server:start`.

## Dependencies

```
composer require doctrine maker security twig
```

## Model

Create a User entity, you can follow the default prompts, use an email as a unique identifier

```
php bin/console make:user
```

don't forget to then create this in the database.

```
php bin/console make:migration
php bin/console doctrine:migrations:migrate
```

## Controller

```
php bin/console make:auth
```

select `1` Login form authenticator; LoginFormAuthenticator; SecurityController; yes;


