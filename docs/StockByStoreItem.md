# StockByStoreItem

Остаток по одному складу в отчете «Остатки по складам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**name** | **str** | Наименование склада | [optional] 
**stock** | **float** | Остаток | [optional] 
**in_transit** | **float** | Ожидание | [optional] 
**reserve** | **float** | Резерв | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.stock_by_store_item import StockByStoreItem

# TODO update the JSON string below
json = "{}"
# create an instance of StockByStoreItem from a JSON string
stock_by_store_item_instance = StockByStoreItem.from_json(json)
# print the JSON string representation of the object
print(StockByStoreItem.to_json())

# convert the object into a dict
stock_by_store_item_dict = stock_by_store_item_instance.to_dict()
# create an instance of StockByStoreItem from a dict
stock_by_store_item_from_dict = StockByStoreItem.from_dict(stock_by_store_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


