# PriceListList

Список Прайс-листов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[PriceList]**](PriceList.md) | Массив Прайс-листов | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.price_list_list import PriceListList

# TODO update the JSON string below
json = "{}"
# create an instance of PriceListList from a JSON string
price_list_list_instance = PriceListList.from_json(json)
# print the JSON string representation of the object
print(PriceListList.to_json())

# convert the object into a dict
price_list_list_dict = price_list_list_instance.to_dict()
# create an instance of PriceListList from a dict
price_list_list_from_dict = PriceListList.from_dict(price_list_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


