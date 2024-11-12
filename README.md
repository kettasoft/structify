# Structify
Structify is a Laravel package that automatically analyzes your application's database schema and generates interactive diagrams to visualize tables, columns, and their relationships. Leveraging the power of Laravel and Vue.js, this package utilizes vue-diagram-editor to provide a dynamic and user-friendly interface, making it easier to understand and manage your database structure.

## Features
- **Schema Extraction:** Automatically retrieves all tables, columns, data types, and foreign key relationships from your database.
- **Interactive Diagrams:** Visualize your database structure with an intuitive and interactive diagram editor powered by `vue-diagram-editor`.
- **Customizable Configuration:** Exclude specific tables, customize diagram styles, and tailor the package to fit your project's needs.
- **API Integration:** Provides API endpoints to fetch schema data, enabling further customization or integration with other tools.

## Installation
1. Require the Package via Composer

```dash
composer require kettasoft/structify
```

2. Publish the Package's Assets and Configuration

```dash
php artisan vendor:publish --provider="Kettasoft\Structify\StructifyServiceProvider"
```

3. Run Migrations (If Applicable)

```dash
php artisan migrate
```

## Usage
1. Include the Blade Component

Add the following Blade component to the view where you want to display the database diagram:
```blade
<x-database-diagram />
```
