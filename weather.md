# Weather API Documentation

## How to use

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