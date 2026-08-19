# StoreSlot

Ячейка склада

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Ячейки склада | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления | [optional] [readonly] 
**name** | **str** | Наименование Ячейки склада | [optional] 
**external_code** | **str** | Внешний код Ячейки склада | [optional] 
**barcode** | **str** | Штрихкод ячейки | [optional] 
**zone** | [**StoreZone**](StoreZone.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.store_slot import StoreSlot

# TODO update the JSON string below
json = "{}"
# create an instance of StoreSlot from a JSON string
store_slot_instance = StoreSlot.from_json(json)
# print the JSON string representation of the object
print(StoreSlot.to_json())

# convert the object into a dict
store_slot_dict = store_slot_instance.to_dict()
# create an instance of StoreSlot from a dict
store_slot_from_dict = StoreSlot.from_dict(store_slot_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


