# StoreZoneList

Список зон Склада

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[StoreZone]**](StoreZone.md) | Массив зон Склада | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.store_zone_list import StoreZoneList

# TODO update the JSON string below
json = "{}"
# create an instance of StoreZoneList from a JSON string
store_zone_list_instance = StoreZoneList.from_json(json)
# print the JSON string representation of the object
print(StoreZoneList.to_json())

# convert the object into a dict
store_zone_list_dict = store_zone_list_instance.to_dict()
# create an instance of StoreZoneList from a dict
store_zone_list_from_dict = StoreZoneList.from_dict(store_zone_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


