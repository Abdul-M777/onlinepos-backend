# Laravel API Backend

This is the backend API for the Vue.js onlinePos, built with Laravel. It provides endpoints for managing restaurant takeaway products.

[Check the live version here](https://abdulmuaz.com/)

## Prerequisites

Ensure you have the following installed:

- [PHP](https://www.php.net/) (8.0+ recommended)
- [Composer](https://getcomposer.org/)
- [MySQL](https://www.mysql.com/) or another database
- [Laravel](https://laravel.com/) (if needed)
- [Node.js](https://nodejs.org/) (for frontend assets, if applicable)

## Installation

1. Clone the repository.

2. Install dependencies:
   ```sh
   composer install
   ```

3. Copy the example environment file and configure it:
   ```sh
   cp .env.example .env
   ```

4. Generate the application key:
   ```sh
   php artisan key:generate
   ```

5. Configure your `.env` file:
   ```
   APP_NAME="Laravel API"
   APP_ENV=local
   APP_KEY=your-generated-key
   APP_DEBUG=true
   APP_URL=http://localhost

   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=your_database
   DB_USERNAME=your_username
   DB_PASSWORD=your_password
   ```

6. Run database migrations:
   ```sh
   php artisan migrate
   ```

## Running the Project

### Development Mode

To start the local server, run:
```sh
php artisan serve
```
By default, the API will be available at `http://127.0.0.1:8000/`.

## Troubleshooting

- If dependencies fail to install, try running:
  ```sh
  rm -rf vendor composer.lock
  composer install
  ```
- If the `.env` file is not loading correctly, run:
  ```sh
  php artisan config:clear
  ```
- Ensure the correct PHP version is installed:
  ```sh
  php -v
  ```

## License

This project is licensed under the MIT License.
