# StockAllList

Расширенный отчет об остатках

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[StockAll]**](StockAll.md) | Массив строк отчета об остатках. Набор типов строк зависит от параметра запроса &#x60;groupBy&#x60; (см. &#x60;meta.type&#x60;: product, variant, consignment).  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.stock_all_list import StockAllList

# TODO update the JSON string below
json = "{}"
# create an instance of StockAllList from a JSON string
stock_all_list_instance = StockAllList.from_json(json)
# print the JSON string representation of the object
print(StockAllList.to_json())

# convert the object into a dict
stock_all_list_dict = stock_all_list_instance.to_dict()
# create an instance of StockAllList from a dict
stock_all_list_from_dict = StockAllList.from_dict(stock_all_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


