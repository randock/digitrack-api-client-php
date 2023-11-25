# # CreateOrderInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference** | **string** | Your order reference. | [optional]
**tracking_number** | **string** | Optional tracking number. If not provided or not unique, we will generate one for you. Must start with your companies unique identifier. | [optional]
**status** | **string** | The status of this order. | [optional] [default to 'created']
**password** | **string** | Optional password that the user will need to supply to see the tracking information. If you are using sequential/numerical tracking numbers, a password is required. | [optional]
**products** | [**\OpenAPI\Client\Model\ProductInput[]**](ProductInput.md) |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
