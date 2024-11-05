Getting started:

[//]: # (database settings are configured in the .env file)
symfony console doctrine:database:create

[//]: # (Create all of the entities with fields)
symfony console make:entity

[//]: # (Create the file used to create the tables from the entities)
symfony console make:migration

[//]: # (Create the tables in the database)
symfony console doctrine:migrations:migrate

[//]: # (Add fixtures to create new data)
symfony console doctrine:fixtures:load
