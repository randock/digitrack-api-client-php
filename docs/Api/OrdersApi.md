# OpenAPI\Client\OrdersApi

All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**create()**](OrdersApi.md#create) | **POST** /orders |  |
| [**delete()**](OrdersApi.md#delete) | **DELETE** /orders/{id} |  |
| [**get()**](OrdersApi.md#get) | **GET** /orders/{id} |  |
| [**getByReference()**](OrdersApi.md#getByReference) | **GET** /orders/by-reference/{reference} |  |
| [**getByTrackingNumber()**](OrdersApi.md#getByTrackingNumber) | **GET** /orders/by-tracking-number/{trackingNumber} |  |
| [**update()**](OrdersApi.md#update) | **PATCH** /orders/{id} |  |


## `create()`

```php
create($create_order_input): \OpenAPI\Client\Model\OrderDto
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$create_order_input = new \OpenAPI\Client\Model\CreateOrderInput(); // \OpenAPI\Client\Model\CreateOrderInput

try {
    $result = $apiInstance->create($create_order_input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->create: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **create_order_input** | [**\OpenAPI\Client\Model\CreateOrderInput**](../Model/CreateOrderInput.md)|  | |

### Return type

[**\OpenAPI\Client\Model\OrderDto**](../Model/OrderDto.md)

### Authorization

[bearer](../../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `delete()`

```php
delete($id)
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new OpenAPI\Client\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 'id_example'; // string

try {
    $apiInstance->delete($id);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->delete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `get()`

```php
get($id): \OpenAPI\Client\Model\OrderDto
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string

try {
    $result = $apiInstance->get($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->get: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\OrderDto**](../Model/OrderDto.md)

### Authorization

[bearer](../../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getByReference()`

```php
getByReference($reference): \OpenAPI\Client\Model\OrderDto
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$reference = 'reference_example'; // string

try {
    $result = $apiInstance->getByReference($reference);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->getByReference: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **reference** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\OrderDto**](../Model/OrderDto.md)

### Authorization

[bearer](../../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getByTrackingNumber()`

```php
getByTrackingNumber($tracking_number, $x_password): \OpenAPI\Client\Model\OrderDto
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new OpenAPI\Client\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$tracking_number = 'tracking_number_example'; // string
$x_password = 'x_password_example'; // string

try {
    $result = $apiInstance->getByTrackingNumber($tracking_number, $x_password);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->getByTrackingNumber: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tracking_number** | **string**|  | |
| **x_password** | **string**|  | [optional] |

### Return type

[**\OpenAPI\Client\Model\OrderDto**](../Model/OrderDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `update()`

```php
update($id, $update_order_input): \OpenAPI\Client\Model\OrderDto
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\OrdersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$update_order_input = new \OpenAPI\Client\Model\UpdateOrderInput(); // \OpenAPI\Client\Model\UpdateOrderInput

try {
    $result = $apiInstance->update($id, $update_order_input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrdersApi->update: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **update_order_input** | [**\OpenAPI\Client\Model\UpdateOrderInput**](../Model/UpdateOrderInput.md)|  | |

### Return type

[**\OpenAPI\Client\Model\OrderDto**](../Model/OrderDto.md)

### Authorization

[bearer](../../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
