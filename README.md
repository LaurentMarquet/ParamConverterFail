# ParamConverterFail
Symfony project to reproduce a test that fails, to be used with [ParamConverterWork](https://github.com/LaurentMarquet/ParamConverterWork)


Project made with the following

```
composer create-project symfony/skeleton ParamConverterFail;

composer require symfony/maker-bundle --dev;

composer require orm;

php bin/console make:entity;

php bin/console make:migration;

php bin/console doctrine:migrations:migrate;

#Added record with SQL `INSERT INTO players VALUES (1);`

php bin/console make:controller;

#Added Route display

composer require --dev symfony/phpunit-bridge;

composer require annotations;

#Added tests

php bin/phpunit;
```