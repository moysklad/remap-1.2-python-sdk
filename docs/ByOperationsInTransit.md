# ByOperationsInTransit

Строка отчета по документам номенклатуры, отображающих ожидания

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assortment** | [**ByOperationsStockAssortment**](ByOperationsStockAssortment.md) |  | [optional] 
**operation** | [**ByOperationsStockOperation**](ByOperationsStockOperation.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**store** | [**ByOperationsStockStore**](ByOperationsStockStore.md) |  | [optional] 
**in_transit** | **float** | Ожидания | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.by_operations_in_transit import ByOperationsInTransit

# TODO update the JSON string below
json = "{}"
# create an instance of ByOperationsInTransit from a JSON string
by_operations_in_transit_instance = ByOperationsInTransit.from_json(json)
# print the JSON string representation of the object
print(ByOperationsInTransit.to_json())

# convert the object into a dict
by_operations_in_transit_dict = by_operations_in_transit_instance.to_dict()
# create an instance of ByOperationsInTransit from a dict
by_operations_in_transit_from_dict = ByOperationsInTransit.from_dict(by_operations_in_transit_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


