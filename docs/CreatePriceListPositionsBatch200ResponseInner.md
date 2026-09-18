# CreatePriceListPositionsBatch200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные номенклатуры, которую представляет собой позиция | [optional] 
**cells** | [**List[PriceListCell]**](PriceListCell.md) | Массив значений столбцов в позиции Прайс-листа | [optional] 
**errors** | [**List[Error]**](Error.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_price_list_positions_batch200_response_inner import CreatePriceListPositionsBatch200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePriceListPositionsBatch200ResponseInner from a JSON string
create_price_list_positions_batch200_response_inner_instance = CreatePriceListPositionsBatch200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreatePriceListPositionsBatch200ResponseInner.to_json())

# convert the object into a dict
create_price_list_positions_batch200_response_inner_dict = create_price_list_positions_batch200_response_inner_instance.to_dict()
# create an instance of CreatePriceListPositionsBatch200ResponseInner from a dict
create_price_list_positions_batch200_response_inner_from_dict = CreatePriceListPositionsBatch200ResponseInner.from_dict(create_price_list_positions_batch200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


