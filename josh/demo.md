# Demo

Instructions for deploying into demo server

## Branch
Always use the `demo` branch for deploying into demo server

## Extra files
It should have following extra files

- `routes/demo.php` - for auto-login user 1
- `resources/views/layouts/_ga.blade.php` - for Google Analytics

## Composer extra installation
Just to avoid polluting existing composer.lock file, we should create a new one for demo server

we need to install package but it should not be added to composer.lock file

```bash
composer require --no-update <package-name>
```

