# PHPUnit

- Install composer
```
composer require --dev phpunit/phpunit
```
- Add the code below in composer.json
```
"autoload": {
        "psr-4":{
            "": "src/"
        }
    }
```
- Run dump-autoload
```
composer dump-autoload
```
- Add phpunit.xml and add the next code
```
<?xml version="1.0" encoding="UTF-8"?>
<phpunit colors="true"
        verbose="true"
        bootstrap="vendor/autoload.php">
        
    <testsuites>
        <testsuite name="Test suite">
            <directory >tests</directory>
        </testsuite>
    </testsuites>

</phpunit>
```

- Add alias to run the tests
```
alias phpunit="./vendor/phpunit/phpunit/phpunit"
```
