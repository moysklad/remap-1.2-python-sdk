# CreateStoreSlotsRequest


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
from moysklad_remap_12_sdk.models.create_store_slots_request import CreateStoreSlotsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateStoreSlotsRequest from a JSON string
create_store_slots_request_instance = CreateStoreSlotsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateStoreSlotsRequest.to_json())

# convert the object into a dict
create_store_slots_request_dict = create_store_slots_request_instance.to_dict()
# create an instance of CreateStoreSlotsRequest from a dict
create_store_slots_request_from_dict = CreateStoreSlotsRequest.from_dict(create_store_slots_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


