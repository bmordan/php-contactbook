# Contactbook

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


