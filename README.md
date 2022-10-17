
# J React Laravel Boilerplate
- This is a react-laravel app using sanctum for authentication and laravel sail.

## Installation
### Installing Project
```bash
- composer create-project nilanth/laravel-react-boilerplate
- cd laravel-react-boilerplate
- Run yarn install
- Create a Database
- Update the Database credential to .env file
- Run php artisan migrate -> To create needed tables.
- Run php artisan db:seed -> To seed some fake users.
- Run yarn run dev OR npm run watch for live updating
- Update API HOST_URL in resources/js/config/constant.js file (For local development change it to 'api')
```
### Installing Sail
```bash
- Download Docker Desktop [https://www.docker.com/products/docker-desktop/]
- If on Windows set up WSL2 development environment [https://learn.microsoft.com/en-us/windows/wsl/setup/environment?source=recommendations]
- Use command 'wsl' to start
- Copy phpunit.xml to root folder
- Install Sail:
    - composer require laravel/sail --dev
    - php artisan sail:install
    - Create alias to use sail command:
        alias sail='[ -f sail ] && sh sail || sh vendor/bin/sail'
- sail up --build -d (this will launch both a mysql and an application docker container to host the Laravel API and the MySql db)
```

### Installing and Connecting to MySQL db
```bash
- download mysql workbench [https://www.mysql.com/products/workbench/]
- Make sure you're not running any other mysql services.
- Create new connection:
    host: 127.0.0.1
    port: 3306
    user: root
    password: password
- create a database and update it in the .env file
```

## Pre-Configured
- Laravel 9
- Laravel Sanctum for SPA Auth
- React 18
- Redux
- React Router
- Route-Level Code-Splitting
- Axios
- Ant Design
- Redux Saga
- Sass
- ESLint
- Preconfigured redux store, actions and saga.

## Plan By Package
[https://github.com/karolkozer/planby]
```bash
yarn add planby
```
