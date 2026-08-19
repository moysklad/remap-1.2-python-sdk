# StoreSlotList

Список ячеек Склада

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[StoreSlot]**](StoreSlot.md) | Массив ячеек Склада | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.store_slot_list import StoreSlotList

# TODO update the JSON string below
json = "{}"
# create an instance of StoreSlotList from a JSON string
store_slot_list_instance = StoreSlotList.from_json(json)
# print the JSON string representation of the object
print(StoreSlotList.to_json())

# convert the object into a dict
store_slot_list_dict = store_slot_list_instance.to_dict()
# create an instance of StoreSlotList from a dict
store_slot_list_from_dict = StoreSlotList.from_dict(store_slot_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


