# InventoryPositionList

Список позиций Инвентаризации

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[InventoryPosition]**](InventoryPosition.md) | Массив позиций Инвентаризации | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.inventory_position_list import InventoryPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of InventoryPositionList from a JSON string
inventory_position_list_instance = InventoryPositionList.from_json(json)
# print the JSON string representation of the object
print(InventoryPositionList.to_json())

# convert the object into a dict
inventory_position_list_dict = inventory_position_list_instance.to_dict()
# create an instance of InventoryPositionList from a dict
inventory_position_list_from_dict = InventoryPositionList.from_dict(inventory_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


