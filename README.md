<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<!-- <p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p> -->

## Laravel 11 Base Template with Jetstream and Livewire

This repository is a **base template** built with **Laravel 11**, preconfigured with **Jetstream** and **Livewire**. It provides a solid foundation for building modern applications with authentication, user management, and dynamic components.

Use this template to quickly create new Laravel projects without having to set up Jetstream and Livewire from scratch.

## Key Features

- **Laravel 11**: The latest version of the Laravel PHP framework.
- **Jetstream**: A starter kit for Laravel applications, including authentication, profile management, and more.
- **Livewire**: Simplifies the creation of dynamic frontend components without writing JavaScript.
- **Authentication**: Includes registration, login, email verification, and password recovery.
- **Dark Mode**: Supports dark mode thanks to Jetstream.

---

## Requirements

Before getting started, ensure you have the following installed in your development environment:

- **PHP 8.2 or higher**
- **Composer** (PHP dependency manager)
- **Node.js** (for frontend asset compilation)
- **SQLite** (or any other Laravel-compatible database system)
- **Git** (optional but recommended)

---

## How to Use This Base Template

Follow these steps to clone this template and create a new project from it:

### 1. Clone the Repository

Clone this repository to your local machine:

```bash
git clone https://github.com/your-username/your-repository.git new-project-name
cd new-project-name
```

### 2. Set Up the New Project

1 - Remove Git History (Optional):
If you want to start with a fresh Git history, delete the .git folder:

```bash
Remove-Item -Recurse -Force .git
```

Then, initialize a new Git repository:

```bash
git init
git add .
git commit -m "Initial commit: New project based on Laravel 11 with Jetstream and Livewire"
```

2 - Install PHP Dependencies:

```bash
composer install
npm install
```

### 3. Configure the .env File

Copy the .env.example file and rename it to .env:

```bash
cp .env.example .env
```

Generate a new application key:

```bash
php artisan key:generate
```

Configure the database in the .env file. For example, for SQLite: (OPTIONAL)

```bash
DB_CONNECTION=sqlite
DB_DATABASE=/absolute/path/to/database.sqlite
```

### 4. Run Migrations

```bash
php artisan migrate
```

### 5. Compile Frontend Assets

```bash
npm run build
```

### 6. Start the Development Server

```bash
php artisan serve
```


### 7. Access the Application:

```bash
http://localhost:8000
```

### Customizing the Project

Once you've cloned and set up the project, you can customize it according to your needs:

## Change the Application Name

Update the application name in the .env file:

```bash
APP_NAME="Your Application Name"
```

## Add New Features

Use Artisan to create new models, controllers, migrations, etc.:

```bash
php artisan make:model ModelName -mcr
```

## Modify Livewire Components

Livewire components are located in resources/views/livewire. You can edit them or create new ones:

```bash
php artisan make:livewire ComponentName
```

### Project Structure

- app/: Contains the application logic (models, controllers, etc.).
- database/: Database migrations and seeders.
- resources/: Views, Livewire components, and frontend assets.
- routes/: Application route definitions.
- config/: Configuration files.

--
## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
