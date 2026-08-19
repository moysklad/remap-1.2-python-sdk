# StoreMetadata

Метаданные складов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**attributes** | [**AttributeMetaInfoList**](AttributeMetaInfoList.md) |  | [optional] 
**create_shared** | **bool** | Создавать новые склады с меткой \&quot;Общий\&quot; | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.store_metadata import StoreMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of StoreMetadata from a JSON string
store_metadata_instance = StoreMetadata.from_json(json)
# print the JSON string representation of the object
print(StoreMetadata.to_json())

# convert the object into a dict
store_metadata_dict = store_metadata_instance.to_dict()
# create an instance of StoreMetadata from a dict
store_metadata_from_dict = StoreMetadata.from_dict(store_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


