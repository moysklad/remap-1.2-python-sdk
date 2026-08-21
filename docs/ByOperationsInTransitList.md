# ByOperationsInTransitList

Отчет по документам номенклатуры, отображающий ожидания

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ByOperationsInTransit]**](ByOperationsInTransit.md) | Массив строк отчета с ожиданиями | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.by_operations_in_transit_list import ByOperationsInTransitList

# TODO update the JSON string below
json = "{}"
# create an instance of ByOperationsInTransitList from a JSON string
by_operations_in_transit_list_instance = ByOperationsInTransitList.from_json(json)
# print the JSON string representation of the object
print(ByOperationsInTransitList.to_json())

# convert the object into a dict
by_operations_in_transit_list_dict = by_operations_in_transit_list_instance.to_dict()
# create an instance of ByOperationsInTransitList from a dict
by_operations_in_transit_list_from_dict = ByOperationsInTransitList.from_dict(by_operations_in_transit_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


