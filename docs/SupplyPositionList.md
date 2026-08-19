# SupplyPositionList

Список позиций Приемки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[SupplyPosition]**](SupplyPosition.md) | Массив позиций Приемки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.supply_position_list import SupplyPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of SupplyPositionList from a JSON string
supply_position_list_instance = SupplyPositionList.from_json(json)
# print the JSON string representation of the object
print(SupplyPositionList.to_json())

# convert the object into a dict
supply_position_list_dict = supply_position_list_instance.to_dict()
# create an instance of SupplyPositionList from a dict
supply_position_list_from_dict = SupplyPositionList.from_dict(supply_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


