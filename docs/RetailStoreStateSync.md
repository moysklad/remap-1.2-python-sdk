# RetailStoreStateSync

Состояние синхронизации

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** | Сообщение | [optional] 
**last_attemp_moment** | **str** | Момент последней попытки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_store_state_sync import RetailStoreStateSync

# TODO update the JSON string below
json = "{}"
# create an instance of RetailStoreStateSync from a JSON string
retail_store_state_sync_instance = RetailStoreStateSync.from_json(json)
# print the JSON string representation of the object
print(RetailStoreStateSync.to_json())

# convert the object into a dict
retail_store_state_sync_dict = retail_store_state_sync_instance.to_dict()
# create an instance of RetailStoreStateSync from a dict
retail_store_state_sync_from_dict = RetailStoreStateSync.from_dict(retail_store_state_sync_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


