# ByOperationsStockList

Отчет по документам номенклатуры, отображающий остатки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ByOperationsStock]**](ByOperationsStock.md) | Массив строк отчета с остатками | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.by_operations_stock_list import ByOperationsStockList

# TODO update the JSON string below
json = "{}"
# create an instance of ByOperationsStockList from a JSON string
by_operations_stock_list_instance = ByOperationsStockList.from_json(json)
# print the JSON string representation of the object
print(ByOperationsStockList.to_json())

# convert the object into a dict
by_operations_stock_list_dict = by_operations_stock_list_instance.to_dict()
# create an instance of ByOperationsStockList from a dict
by_operations_stock_list_from_dict = ByOperationsStockList.from_dict(by_operations_stock_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


