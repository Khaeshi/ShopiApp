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

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- **PHP** 8.2 or higher
- **Composer** (PHP package manager)
- **Node.js** 18+ and **npm**
- **Git**

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd ShopiApp
   ```

2. **Install PHP dependencies**
   ```bash
   composer install
   ```

3. **Install Node.js dependencies**
   ```bash
   npm install
   ```

4. **Environment setup**
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

5. **Database setup**
   ```bash
   # For development (SQLite)
   touch database/database.sqlite
   php artisan migrate
   
   # For production (MySQL/PostgreSQL)
   # Update .env with your database credentials
   php artisan migrate
   ```

6. **Build assets**
   ```bash
   npm run build
   ```

## 🏃‍♂️ Development

### Starting the development server

The project includes a convenient development script that runs all services concurrently:

```bash
composer run dev
```

This will start:
- Laravel development server
- Vite dev server (React hot reload)
- Queue worker
- File watchers

### Alternative development commands

```bash
# Laravel server only
php artisan serve

# Vite dev server only
npm run dev

# Build for production
npm run build

# Run tests
composer test
# or
php artisan test

# Code formatting
npm run format
composer pint

# Linting
npm run lint
```

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

## 🚀 Deployment

### Production Build

1. **Install dependencies**
   ```bash
   composer install --optimize-autoloader --no-dev
   npm ci
   npm run build
   ```

2. **Environment setup**
   ```bash
   cp .env.example .env
   # Edit .env with production settings
   php artisan key:generate
   ```

3. **Database setup**
   ```bash
   php artisan migrate --force
   ```

4. **Cache optimization**
   ```bash
   php artisan config:cache
   php artisan route:cache
   php artisan view:cache
   ```

## 📝 Available Scripts

### Composer Scripts
- `composer dev` - Start development environment
- `composer dev:ssr` - Start with SSR enabled
- `composer test` - Run tests

### NPM Scripts
- `npm run dev` - Start Vite dev server
- `npm run build` - Build for production
- `npm run build:ssr` - Build with SSR
- `npm run format` - Format code with Prettier
- `npm run lint` - Lint code with ESLint
- `npm run types` - Type checking

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

If you encounter any issues or have questions:

1. Check the [Laravel documentation](https://laravel.com/docs)
2. Check the [React documentation](https://react.dev)
3. Open an issue in this repository

---

**Happy coding! 🎉** 