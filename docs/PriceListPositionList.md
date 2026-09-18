# PriceListPositionList

Список позиций Прайс-листа

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[PriceListPosition]**](PriceListPosition.md) | Массив позиций Прайс-листа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.price_list_position_list import PriceListPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of PriceListPositionList from a JSON string
price_list_position_list_instance = PriceListPositionList.from_json(json)
# print the JSON string representation of the object
print(PriceListPositionList.to_json())

# convert the object into a dict
price_list_position_list_dict = price_list_position_list_instance.to_dict()
# create an instance of PriceListPositionList from a dict
price_list_position_list_from_dict = PriceListPositionList.from_dict(price_list_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


