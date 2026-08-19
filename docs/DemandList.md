# DemandList

Список Отгрузок

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Demand]**](Demand.md) | Массив Отгрузок | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.demand_list import DemandList

# TODO update the JSON string below
json = "{}"
# create an instance of DemandList from a JSON string
demand_list_instance = DemandList.from_json(json)
# print the JSON string representation of the object
print(DemandList.to_json())

# convert the object into a dict
demand_list_dict = demand_list_instance.to_dict()
# create an instance of DemandList from a dict
demand_list_from_dict = DemandList.from_dict(demand_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


