# ByOperationsStockStore

Метаданные склада документа

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.by_operations_stock_store import ByOperationsStockStore

# TODO update the JSON string below
json = "{}"
# create an instance of ByOperationsStockStore from a JSON string
by_operations_stock_store_instance = ByOperationsStockStore.from_json(json)
# print the JSON string representation of the object
print(ByOperationsStockStore.to_json())

# convert the object into a dict
by_operations_stock_store_dict = by_operations_stock_store_instance.to_dict()
# create an instance of ByOperationsStockStore from a dict
by_operations_stock_store_from_dict = ByOperationsStockStore.from_dict(by_operations_stock_store_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


