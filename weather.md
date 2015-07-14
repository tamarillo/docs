# Weather API Documentation

## How to use

```php
<?php

// Composer Autoloader
require_once 'vendor/autoload.php';

// The Location for Stuttgart, Germany
$weather = Tamarillo\Weather\Weather::getWeather([ 48.782318, 9.17702 ];

echo $wether->weather()->id();    // The ID of the current weather

echo $wether->city();             // The name of the City
echo $wether->city()->id();       // The ID of the City
var_dump($wether->geo());         // An array of the coordinations of the City

echo $wether->weather();          // The current weather description
echo $wether->weather()->icon();  // The current weather icon
```

### Get weather information for today

```php
// By geographic coordinats
$info = Weather::today(48.779209,9.1772152);

// By city name
$info = Weather::today('Stuttgart');

// By city ID
$info = Weather::today(2825297);
```

Where the city ID is the ID for the city you will get as an information in each request.

### Get the city ID
```php
$cityID = Weather::findCity('Stuttgart'); // 2825297
```


#### Note
We actual build der Version 1.0 and will submit it soon to GitHub. Whe are sorry for that.