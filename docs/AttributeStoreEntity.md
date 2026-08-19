# AttributeStoreEntity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | [**Store**](Store.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_store_entity import AttributeStoreEntity

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeStoreEntity from a JSON string
attribute_store_entity_instance = AttributeStoreEntity.from_json(json)
# print the JSON string representation of the object
print(AttributeStoreEntity.to_json())

# convert the object into a dict
attribute_store_entity_dict = attribute_store_entity_instance.to_dict()
# create an instance of AttributeStoreEntity from a dict
attribute_store_entity_from_dict = AttributeStoreEntity.from_dict(attribute_store_entity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


