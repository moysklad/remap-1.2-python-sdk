# AttributeProjectEntity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | [**Project**](Project.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_project_entity import AttributeProjectEntity

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeProjectEntity from a JSON string
attribute_project_entity_instance = AttributeProjectEntity.from_json(json)
# print the JSON string representation of the object
print(AttributeProjectEntity.to_json())

# convert the object into a dict
attribute_project_entity_dict = attribute_project_entity_instance.to_dict()
# create an instance of AttributeProjectEntity from a dict
attribute_project_entity_from_dict = AttributeProjectEntity.from_dict(attribute_project_entity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


