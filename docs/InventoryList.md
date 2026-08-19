# InventoryList

Список Инвентаризаций

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Inventory]**](Inventory.md) | Массив Инвентаризаций | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.inventory_list import InventoryList

# TODO update the JSON string below
json = "{}"
# create an instance of InventoryList from a JSON string
inventory_list_instance = InventoryList.from_json(json)
# print the JSON string representation of the object
print(InventoryList.to_json())

# convert the object into a dict
inventory_list_dict = inventory_list_instance.to_dict()
# create an instance of InventoryList from a dict
inventory_list_from_dict = InventoryList.from_dict(inventory_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


