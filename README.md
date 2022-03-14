```
composer create project daniels/fuellogger-project
```

complete .env file (from .env.example template)

```
./vendor/bin/doctrine-migrations migrations:migrate --configuration ./src/Migrations/migrations.php --db-configuration ./src/Migrations/migrations_db.php
```