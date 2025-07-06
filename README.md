# ShopiApp

A modern e-commerce application built with Laravel and React, featuring a beautiful UI with Tailwind CSS and TypeScript.

## 🚀 Tech Stack

- **Backend**: Laravel 12.x (PHP 8.2+)
- **Frontend**: React 19.x with TypeScript
- **Styling**: Tailwind CSS 4.x
- **UI Components**: Radix UI + Headless UI
- **Build Tool**: Vite
- **Database**: SQLite (development) / MySQL/PostgreSQL (production)
- **Testing**: Pest PHP


## 📁 Project Structure

```
ShopiApp/
├── app/                    # Laravel application logic
├── resources/
│   ├── js/                # React components and pages
│   └── css/               # Stylesheets
├── routes/                # Laravel routes
├── database/              # Migrations, seeders, factories
├── tests/                 # Test files
├── public/                # Public assets
├── config/                # Laravel configuration
├── storage/               # File storage
├── vendor/                # Composer dependencies
├── node_modules/          # npm dependencies
└── .github/               # GitHub workflows
```

## 🧪 Testing

The project uses Pest PHP for testing:

```bash
# Run all tests
composer test

# Run tests with coverage
composer test -- --coverage

# Run specific test file
php artisan test tests/Feature/ExampleTest.php
```


## 📄 License

This project is licensed under the MIT License - see the [NOTICE](NOTICE.md) file for details.


