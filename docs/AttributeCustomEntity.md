# AttributeCustomEntity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | [**CustomEntityElement**](CustomEntityElement.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_custom_entity import AttributeCustomEntity

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeCustomEntity from a JSON string
attribute_custom_entity_instance = AttributeCustomEntity.from_json(json)
# print the JSON string representation of the object
print(AttributeCustomEntity.to_json())

# convert the object into a dict
attribute_custom_entity_dict = attribute_custom_entity_instance.to_dict()
# create an instance of AttributeCustomEntity from a dict
attribute_custom_entity_from_dict = AttributeCustomEntity.from_dict(attribute_custom_entity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


