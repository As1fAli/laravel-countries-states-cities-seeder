# Laravel Countries States Cities Seeder
Laravel migrations and seeders for countries, states and cities tables


## Introduction
Packages are great, but they also make us dependant on them. We have to register their service providers into application and code according to their documentation even when we can achieve that task without these.

At least for myself, I found it very overwhelming when it comes to create countries, states and cities tables from laravel migrations and seed them. So I created migrations and seeders for that purpose using two popular repositories (mentioned in credits).

### Note
This is not package, this just includes countries, states, cities migrations and seeders files. You are free to use standard Laravel relationships and code for your project.

## Requirements
* PHP 7 OR Above
* Laravel 7 or Above
* memory_limit of PHP running in terminal should be 350MB or Above.

# Installation
1. in your php.ini file, set your memory_limit to 350MB
    `
    memory_limit = 350M
    `
2. If you face memory exuasted error, increase that limit.
```
You can revert this change after seeding is completed.
```
5. clone repository in your laravel project

## Credits
* [Inverse seed generator (iSeed)](https://github.com/orangehill/iseed)
* [Countries States Cities Database](https://github.com/dr5hn/countries-states-cities-database)
