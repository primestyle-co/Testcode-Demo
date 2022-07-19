<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

## UnitTest Laravel
depend on each project level, can implement unit test more or less, Laravel Testing can test Mode, Service, Mail, Controller, Helper, Console... whenever you create or update funtion you must write test for it. But it will take lots of time
In this project I only make unit test for Controller. It a minimum requirements.

### implement
make a copy of the .env -> .env.testing
you can edit setting by edit phpunit.xml (but i think better leave it as default)
edit .env.testing change Database
DB_DATABASE=example_test
DB_USERNAME=root
DB_PASSWORD=

### Write UnitTest and Run
Create test file in this folder tests/Feature/
You can refer to this file tests/Feature/Http/Controllers/PostControllerTest.php
### Run UnitTest
run all test php artisan test --testsuite=Feature
run one file php artisan test --testsuite=Feature 'tests/Feature/Http/Controllers/PostControllerTest.php'
run one function in file php artisan test --testsuite=Feature --filter 'testIndexFailWithoutAuth' 'tests/Feature/Http/Controllers/PostControllerTest.php'

you can refer this link below it very clear and detailed.
https://laravel.com/docs/9.x/testing

## UnitTest Vue
not yet implement.
