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

# Installation
1. Clone repository and move migrations and seeders into relevant directories.
2. Register Seeders into `database/seeders/DatabaseSeeder.php` by adding these line in run method
```
$this->call(CountriesTableSeeder::class);
$this->call(StatesTableSeeder::class);
$this->call(CitiesTableChunkOneSeeder::class);
$this->call(CitiesTableChunkTwoSeeder::class);
$this->call(CitiesTableChunkThreeSeeder::class);
$this->call(CitiesTableChunkFourSeeder::class);
$this->call(CitiesTableChunkFiveSeeder::class);
```
3. Run your migrations.
5. Seed the data using `php -d memory_limit=350M artisan db:seed` command
```
If You face memory exausted error, increase value of memory_limit in this command.
```

## Credits
* [Inverse seed generator (iSeed)](https://github.com/orangehill/iseed)
* [Countries States Cities Database](https://github.com/dr5hn/countries-states-cities-database)
