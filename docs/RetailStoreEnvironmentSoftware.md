# RetailStoreEnvironmentSoftware

Информация о ПО

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Наименование ПО | [optional] 
**vendor** | **str** | Производитель ПО | [optional] 
**version** | **str** | Версия ПО | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_store_environment_software import RetailStoreEnvironmentSoftware

# TODO update the JSON string below
json = "{}"
# create an instance of RetailStoreEnvironmentSoftware from a JSON string
retail_store_environment_software_instance = RetailStoreEnvironmentSoftware.from_json(json)
# print the JSON string representation of the object
print(RetailStoreEnvironmentSoftware.to_json())

# convert the object into a dict
retail_store_environment_software_dict = retail_store_environment_software_instance.to_dict()
# create an instance of RetailStoreEnvironmentSoftware from a dict
retail_store_environment_software_from_dict = RetailStoreEnvironmentSoftware.from_dict(retail_store_environment_software_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


