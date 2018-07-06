# Формат запроса

Обращение к сервису производится с помощью метода GET по протоколу HTTP. URL сервиса имеет вид:

```text
https://api.oasiscatalog.com/v3/[тип_выгрузки]?[параметр=значение]
```

, где

* [https://api.oasiscatalog.com](https://api.oasiscatalog.com) - URL API-сервиса Oasis
* v3 - текущая версия API
* \[тип выгрузки\] - тип выгрузки
* ?\[параметр=значение\] - дополнительные параметры запроса

Также, есть возможность выгрузки в виде файла:

```text
https://api.oasiscatalog.com/v3/[тип_выгрузки]/download?[format=xml|json]
```

, где

* [https://api.oasiscatalog.com](https://api.oasiscatalog.com) - URL API-сервиса Oasis
* v3 - текущая версия API
* \[тип выгрузки\] - тип выгрузки
* ?\[format=xml\|json\] - формат данных xml или json

## Пример

Фрагмент кода на PHP, который отправляет запрос к сервису с помощью технологии [CURL](http://ru.wikipedia.org/wiki/CURL). В примере показан разбор полученного ответа на заголовки и непосредственно тело ответа.

```php
$apiKey = 'yourAPIkeyHERE'; // Ваш ключ доступа
    $apiUrl = 'https://api.oasiscatalog.com/v3/stock'; // URL для выгрузки остатков
    $headers = [
        'Accept:application/xml', // получить выгрузку в формате XML
    ];

    $resource = curl_init();

    curl_setopt_array($resource, [
        CURLOPT_URL => $apiUrl, // URL текущего запроса к сервису
        CURLOPT_HEADER => true, // указать сервису включить заголовки в ответ
        CURLOPT_HTTPHEADER => $headers, // массив заголовков для отправки запроса
        CURLOPT_RETURNTRANSFER => true,
        CURLOPT_USERPWD => $apiKey, // ключ доступа
        CURLOPT_TIMEOUT => 30,
    ]);

    $response = curl_exec($resource);

    $headerSize = curl_getinfo($resource, CURLINFO_HEADER_SIZE);
    $header = substr($response, 0, $header_size); // отделяем заголовки ответа
    $body = substr($response, $header_size); // сохраняем непосредственно тело ответа

    curl_close($resource);

    // далее извлекаем из переменной $body массив данных, согласно запрошенному формату (XML или JSON)
```

