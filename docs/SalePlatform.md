# SalePlatform

Площадка для продаж

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Площадки для продаж | [optional] [readonly] 
**name** | **str** | Наименование Площадки для продаж | [optional] 
**sale_platform_group** | **str** | Группа площадок для продаж. Известные значения описаны в SalePlatformGroup | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.sale_platform import SalePlatform

# TODO update the JSON string below
json = "{}"
# create an instance of SalePlatform from a JSON string
sale_platform_instance = SalePlatform.from_json(json)
# print the JSON string representation of the object
print(SalePlatform.to_json())

# convert the object into a dict
sale_platform_dict = sale_platform_instance.to_dict()
# create an instance of SalePlatform from a dict
sale_platform_from_dict = SalePlatform.from_dict(sale_platform_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


