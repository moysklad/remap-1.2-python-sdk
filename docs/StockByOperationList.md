# StockByOperationList

Отчет «Остатки по документам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[StockByOperation]**](StockByOperation.md) | Массив строк отчета с остатками по документам | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.stock_by_operation_list import StockByOperationList

# TODO update the JSON string below
json = "{}"
# create an instance of StockByOperationList from a JSON string
stock_by_operation_list_instance = StockByOperationList.from_json(json)
# print the JSON string representation of the object
print(StockByOperationList.to_json())

# convert the object into a dict
stock_by_operation_list_dict = stock_by_operation_list_instance.to_dict()
# create an instance of StockByOperationList from a dict
stock_by_operation_list_from_dict = StockByOperationList.from_dict(stock_by_operation_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


