# ByOperationsReserve

Строка отчета по документам номенклатуры, отображающего резервы

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assortment** | [**ByOperationsStockAssortment**](ByOperationsStockAssortment.md) |  | [optional] 
**operation** | [**ByOperationsStockOperation**](ByOperationsStockOperation.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**store** | [**ByOperationsStockStore**](ByOperationsStockStore.md) |  | [optional] 
**reserve** | **float** | Резерв | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.by_operations_reserve import ByOperationsReserve

# TODO update the JSON string below
json = "{}"
# create an instance of ByOperationsReserve from a JSON string
by_operations_reserve_instance = ByOperationsReserve.from_json(json)
# print the JSON string representation of the object
print(ByOperationsReserve.to_json())

# convert the object into a dict
by_operations_reserve_dict = by_operations_reserve_instance.to_dict()
# create an instance of ByOperationsReserve from a dict
by_operations_reserve_from_dict = ByOperationsReserve.from_dict(by_operations_reserve_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


