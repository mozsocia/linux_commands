To install PHP and set up Laravel with SQLite for development on Ubuntu, follow these steps:

### Step 1: Update your package list
First, update your package list to ensure you have the latest information about available packages:
```bash
sudo apt update
```

### Step 2: Install PHP and required extensions
Install PHP along with the necessary extensions for Laravel and SQLite:
```bash
sudo apt install php php-cli php-mbstring php-xml php-zip php-sqlite3
```

### Step 3: Install Composer
Composer is a dependency manager for PHP, which is required to install Laravel:
```bash
sudo apt install composer
```

### Step 4: Install Laravel via Composer
You can install Laravel globally using Composer, or you can create a new Laravel project. Here we'll create a new Laravel project:
```bash
composer create-project --prefer-dist laravel/laravel your_project_name
```
Replace `your_project_name` with the desired name of your Laravel project.

### Step 5: Configure SQLite for Laravel
Laravel supports SQLite out of the box. You'll need to create an SQLite database file and update your `.env` file to use SQLite.

1. Create a new SQLite database file:
   ```bash
   touch database/database.sqlite
   ```

2. Open the `.env` file in the root of your Laravel project and set the following database configuration:
   ```env
   DB_CONNECTION=sqlite
   DB_DATABASE=/full/path/to/your/project/database/database.sqlite
   ```
   Replace `/full/path/to/your/project` with the actual path to your Laravel project.

### Step 6: Generate application key
Laravel requires an application key to be set, which is used for encryption purposes. You can generate this key using the Artisan command-line tool:
```bash
php artisan key:generate
```

### Step 7: Serve the Laravel application
You can use the built-in PHP server to serve your Laravel application during development:
```bash
php artisan serve
```
By default, this will start the server at `http://127.0.0.1:8000`.

### Summary of Commands
Here is a summary of all the commands:
```bash
sudo apt update
sudo apt install php php-cli php-mbstring php-xml php-zip php-sqlite3
sudo apt install composer
composer create-project --prefer-dist laravel/laravel your_project_name
cd your_project_name
touch database/database.sqlite
php artisan key:generate
php artisan serve
```

After running these commands, your Laravel application should be set up and running with SQLite on your Ubuntu system.
