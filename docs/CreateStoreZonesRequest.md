# CreateStoreZonesRequest


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
from moysklad_remap_12_sdk.models.create_store_zones_request import CreateStoreZonesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateStoreZonesRequest from a JSON string
create_store_zones_request_instance = CreateStoreZonesRequest.from_json(json)
# print the JSON string representation of the object
print(CreateStoreZonesRequest.to_json())

# convert the object into a dict
create_store_zones_request_dict = create_store_zones_request_instance.to_dict()
# create an instance of CreateStoreZonesRequest from a dict
create_store_zones_request_from_dict = CreateStoreZonesRequest.from_dict(create_store_zones_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


