# DemandPositionList

Список позиций Отгрузки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[DemandPosition]**](DemandPosition.md) | Массив позиций Отгрузки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.demand_position_list import DemandPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of DemandPositionList from a JSON string
demand_position_list_instance = DemandPositionList.from_json(json)
# print the JSON string representation of the object
print(DemandPositionList.to_json())

# convert the object into a dict
demand_position_list_dict = demand_position_list_instance.to_dict()
# create an instance of DemandPositionList from a dict
demand_position_list_from_dict = DemandPositionList.from_dict(demand_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


