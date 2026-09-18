# PriceListPosition

Позиция Прайс-листа

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные номенклатуры, которую представляет собой позиция | [optional] 
**cells** | [**List[PriceListCell]**](PriceListCell.md) | Массив значений столбцов в позиции Прайс-листа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.price_list_position import PriceListPosition

# TODO update the JSON string below
json = "{}"
# create an instance of PriceListPosition from a JSON string
price_list_position_instance = PriceListPosition.from_json(json)
# print the JSON string representation of the object
print(PriceListPosition.to_json())

# convert the object into a dict
price_list_position_dict = price_list_position_instance.to_dict()
# create an instance of PriceListPosition from a dict
price_list_position_from_dict = PriceListPosition.from_dict(price_list_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


