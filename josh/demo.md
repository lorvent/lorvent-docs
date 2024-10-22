# Demo

Instructions for deploying into demo server

## Installation

### cyberpanel

#### login as josha2140

first we should login as current user
``` sudo su josha2140```

assuming php version is `8.2` and 
`composer` is located at `/usr/bin/composer`, 

then we need to run php with following command

 ```/usr/local/lsws/lsphp82/bin/php```

example: to run composer install
```bash
/usr/local/lsws/lsphp82/bin/php /usr/bin/composer install
```


example: php artisan migrate
```bash
/usr/local/lsws/lsphp82/bin/php artisan migrate
``` 

## Branch
Always use the `demo` branch for deploying into demo server

## Dummy Data

### users

```bash
/usr/local/lsws/lsphp82/bin/php artisan db:seed --class=UsersSeeder
```

### all other data

```
/usr/local/lsws/lsphp82/bin/php artisan db:seed --class=DemoSeeder
```

