```
composer create project daniels/fuellogger-project
```

complete .env file

```
./vendor/bin/doctrine-migrations migrations:migrate --configuration ./src/Migrations/migrations.php --db-configuration ./src/Migrations/migrations_db.php
```