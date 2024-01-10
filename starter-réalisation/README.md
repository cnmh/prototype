# Starter réalisation
## Packages

1. Laravel ui adminlte
[infyom.com](https://infyom.com/open-source/laravel-ui-adminlte/docs)

```bash
composer require infyomlabs/laravel-ui-adminlte
```
```bash
php artisan ui adminlte --auth
```
```bash
npm install
npm run build
```
## Réalisation

### .env

```
DB_DATABASE=starter_realisation
DB_USERNAME=root
DB_PASSWORD=solicoders
```

### Seeders
```php
class DatabaseSeeder extends Seeder
{
    public function run(): void
    {
        \App\Models\User::factory()->create([
            'name' => 'admin',
            'email' => 'admin@example.com',
        ]);
    }
}
```
### Exécuter des migrations et seeders

```bash
php artisan migrate --seed
```
