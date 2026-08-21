# ByOperationsReserveList

Отчет по документам номенклатуры, отображающий резервы

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ByOperationsReserve]**](ByOperationsReserve.md) | Массив строк отчета с резервами | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.by_operations_reserve_list import ByOperationsReserveList

# TODO update the JSON string below
json = "{}"
# create an instance of ByOperationsReserveList from a JSON string
by_operations_reserve_list_instance = ByOperationsReserveList.from_json(json)
# print the JSON string representation of the object
print(ByOperationsReserveList.to_json())

# convert the object into a dict
by_operations_reserve_list_dict = by_operations_reserve_list_instance.to_dict()
# create an instance of ByOperationsReserveList from a dict
by_operations_reserve_list_from_dict = ByOperationsReserveList.from_dict(by_operations_reserve_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


