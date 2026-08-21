# StockByStoreList

Отчет «Остатки по складам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[StockByStore]**](StockByStore.md) | Массив строк отчета. Набор типов строк зависит от параметра запроса &#x60;groupBy&#x60; (см. &#x60;meta.type&#x60;: product, variant, consignment).  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.stock_by_store_list import StockByStoreList

# TODO update the JSON string below
json = "{}"
# create an instance of StockByStoreList from a JSON string
stock_by_store_list_instance = StockByStoreList.from_json(json)
# print the JSON string representation of the object
print(StockByStoreList.to_json())

# convert the object into a dict
stock_by_store_list_dict = stock_by_store_list_instance.to_dict()
# create an instance of StockByStoreList from a dict
stock_by_store_list_from_dict = StockByStoreList.from_dict(stock_by_store_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


