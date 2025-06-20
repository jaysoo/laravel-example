# Laravel Monorepo

This is a basic Laravel monorepo structure using Composer.

## Structure

```
./
├── apps/
│   └── laravel-app/    # Main Laravel application
├── packages/           # Shared packages
├── shared/            # Shared resources
├── composer.json      # Monorepo root composer configuration
└── README.md
```

## Getting Started

1. Install dependencies:
```bash
composer install
```

2. Run the Laravel application:
```bash
cd apps/laravel-app
php artisan serve
```

## Adding New Packages

To add new packages to the monorepo, create them in the `packages/` directory and update the root `composer.json` to include them in the PSR-4 autoloading.

## Testing

Run tests from the monorepo root:
```bash
composer test
```
