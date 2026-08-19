# SalePlatformList

Список площадок для продаж

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[SalePlatform]**](SalePlatform.md) | Массив площадок для продаж | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.sale_platform_list import SalePlatformList

# TODO update the JSON string below
json = "{}"
# create an instance of SalePlatformList from a JSON string
sale_platform_list_instance = SalePlatformList.from_json(json)
# print the JSON string representation of the object
print(SalePlatformList.to_json())

# convert the object into a dict
sale_platform_list_dict = sale_platform_list_instance.to_dict()
# create an instance of SalePlatformList from a dict
sale_platform_list_from_dict = SalePlatformList.from_dict(sale_platform_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


