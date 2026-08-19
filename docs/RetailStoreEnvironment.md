# RetailStoreEnvironment

Информация о среде (оборудование, ПО и т.д.)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**device** | **str** | Устройство | [optional] 
**os** | **str** | Операционная система | [optional] 
**software** | [**RetailStoreEnvironmentSoftware**](RetailStoreEnvironmentSoftware.md) |  | [optional] 
**cheque_printer** | [**RetailStoreEnvironmentChequePrinter**](RetailStoreEnvironmentChequePrinter.md) |  | [optional] 
**payment_terminal** | **str** | Терминал оплаты | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_store_environment import RetailStoreEnvironment

# TODO update the JSON string below
json = "{}"
# create an instance of RetailStoreEnvironment from a JSON string
retail_store_environment_instance = RetailStoreEnvironment.from_json(json)
# print the JSON string representation of the object
print(RetailStoreEnvironment.to_json())

# convert the object into a dict
retail_store_environment_dict = retail_store_environment_instance.to_dict()
# create an instance of RetailStoreEnvironment from a dict
retail_store_environment_from_dict = RetailStoreEnvironment.from_dict(retail_store_environment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


