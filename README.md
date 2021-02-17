## What does the application do?
Central application creates a new site and add admins and modules for this created site. 

- [Requirements](#requirements)
- [Installation](#installation)
- [Structure](#structure)
- [DB design](#db-design)
- [How system works](#how-system-works)
- [Unit test](#unit-test)

## Requirements 
* PHP version: 7.3 at least 
* Laravel framework version: 7
* Database type: Mysql 
* Mysql version: 8.0.18
* Linux server

## Installation
* Read installation: [Here](DOC/installation.md).
  
## Structure
* Read structure: [Here](DOC/structure.md).

## DB design 
* Read [DB design](DOC/design.md).

## How system works 
* Read [Cycle](DOC/cycle.md).
  
## Unit test
* In TDD we use phpunit as unit test for each units to application.
* The unit testing falled into path `tests` directory which contains two directory.
* The first is `Feature` for test full feature for module.
* The second is `Unit` for test small unit for module.
* In common we use `Feature` directory for test application.
* Every module have test file for it.
* To run specific class execute either of two following commands.

```php 
"./vendor/bin/phpunit" --filter UnitTestClassName
```
```php 
php artisan test --filter UnitTestClassName
```

* To run specific method execute either of two following commands.
```php 
"./vendor/bin/phpunit" --filter MethodName
```
```php 
php artisan test --filter MethodName
```
   
* To run all unit test execute either of two following commands.
```php 
php artisan test
```
```php 
"./vendor/bin/phpunit"
```
* To Export report for test execute following command.
```php 
./vendor/bin/phpunit --coverage-html ReportPath
```





