# php-curl
PHP curl class wrapper

# Installation
```
composer require vesic/php-curl
```

# Usage
```
use \Vesic\Curl\Curl;

$curl = Curl::getCurlObject();
$curl = Curl::getCurlObject('http://www.example.com');

$curl->setUrl('http://www.example.com');

$curl->setOption('url', 'https://jsonplaceholder.typicode.com/users/1');

$curl->setOptionsArray(['url'=>'https://jsonplaceholder.typicode.com/users/1', 'file'=>'json.txt']);

$response = $curl->exec(false); // write to the stdout
```
