Make sure that Composer is available.

Create the project with this command:

```
composer create-project daniels/fuellogger-project mypath dev-main
```

Create and complete the `.env` file from the template `.env.example`.

```
./vendor/bin/doctrine-migrations migrations:migrate --configuration ./src/Migrations/migrations.php --db-configuration ./src/Migrations/migrations_db.php
```

Set up Basic Auth password protection for the entire root directory. Required files and folders are excluded from Basic Auth per default.

Then install the following cronjobs:

from these shell calls
```
/.../bin/fuelPricesCron  (recommended interval of 7 minutes)
/.../bin/oilPricesCron   (recommended interval of 24 hours)
```

or alternatively via these public URLs (use Basic Auth credentials)
```
https://my.url.dev/Public/fuelPricesCron.php   (recommended interval of 7 minutes)
https://my.url.dev/Public/oilPricesCron.php    (recommended interval of 24 hours)
```

Set your domain document root to the `src` directory.
