# Laravel Template

### Features:
- Using Laravel Sail(docker-compose) and a bunch of pre-configured services:
  - MySQL
  - PhpMyAdmin
  - Redis
  - Mailhog
  - Minio
  - MeiliSearch
  - Swagger-UI
- PHP-CS-Fixer to automatically fix code using `@PSR12` and `@PSR12:risky` rule sets.
- Larastan(PhpStan)
- Running fix, test, analyze and unify-docs before any commit using `.githooks/pre-commit`

### Available Commands:
- `composer fix`: run php-cs-fixer for the whole project
- `composer test`: alias of `php artisan test`
- `composer analyze`: run phpstan for the whole project
- `npm run unify-docs`: bundle up all openapi files into one big yaml and json file

### Notes

Configure git on your system to look for hooks in the `.githooks` directory instead of the deafult `.git/hooks` directory. You can run `git config core.hooksPath .githooks` for this.

Laravel Sail is used for development, follow the guide in the [documentation](https://laravel.com/docs/9.x/sail#configuring-a-bash-alias) to use it
