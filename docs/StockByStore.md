# StockByStore

Строка отчета «Остатки по складам».  Тип номенклатуры в строке задается `meta.type` (product, variant или consignment). Параметр запроса `groupBy` определяет набор возможных типов в выдаче: `product` — только товары; `variant` — товары и модификации; `consignment` — товары, модификации и партии. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**stock_by_store** | [**List[StockByStoreItem]**](StockByStoreItem.md) | Остатки по складам. Размерность массива равна количеству складов в системе.  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.stock_by_store import StockByStore

# TODO update the JSON string below
json = "{}"
# create an instance of StockByStore from a JSON string
stock_by_store_instance = StockByStore.from_json(json)
# print the JSON string representation of the object
print(StockByStore.to_json())

# convert the object into a dict
stock_by_store_dict = stock_by_store_instance.to_dict()
# create an instance of StockByStore from a dict
stock_by_store_from_dict = StockByStore.from_dict(stock_by_store_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


