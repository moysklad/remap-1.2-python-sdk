# StoreZone

Зона склада

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Зоны склада | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления | [optional] [readonly] 
**name** | **str** | Наименование Зоны склада | [optional] 
**external_code** | **str** | Внешний код Зоны склада | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.store_zone import StoreZone

# TODO update the JSON string below
json = "{}"
# create an instance of StoreZone from a JSON string
store_zone_instance = StoreZone.from_json(json)
# print the JSON string representation of the object
print(StoreZone.to_json())

# convert the object into a dict
store_zone_dict = store_zone_instance.to_dict()
# create an instance of StoreZone from a dict
store_zone_from_dict = StoreZone.from_dict(store_zone_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


