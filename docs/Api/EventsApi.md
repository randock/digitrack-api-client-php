# OpenAPI\Client\EventsApi

All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**eventControllerAddEvent()**](EventsApi.md#eventControllerAddEvent) | **POST** /events |  |
| [**eventControllerDeleteEvent()**](EventsApi.md#eventControllerDeleteEvent) | **DELETE** /events/{id} |  |


## `eventControllerAddEvent()`

```php
eventControllerAddEvent($create_event_input): \OpenAPI\Client\Model\EventDto
```



Creates a new event.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\EventsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$create_event_input = new \OpenAPI\Client\Model\CreateEventInput(); // \OpenAPI\Client\Model\CreateEventInput

try {
    $result = $apiInstance->eventControllerAddEvent($create_event_input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventsApi->eventControllerAddEvent: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **create_event_input** | [**\OpenAPI\Client\Model\CreateEventInput**](../Model/CreateEventInput.md)|  | |

### Return type

[**\OpenAPI\Client\Model\EventDto**](../Model/EventDto.md)

### Authorization

[bearer](../../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `eventControllerDeleteEvent()`

```php
eventControllerDeleteEvent($id)
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\EventsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string

try {
    $apiInstance->eventControllerDeleteEvent($id);
} catch (Exception $e) {
    echo 'Exception when calling EventsApi->eventControllerDeleteEvent: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

void (empty response body)

### Authorization

[bearer](../../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
