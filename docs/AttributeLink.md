# AttributeLink


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_link import AttributeLink

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeLink from a JSON string
attribute_link_instance = AttributeLink.from_json(json)
# print the JSON string representation of the object
print(AttributeLink.to_json())

# convert the object into a dict
attribute_link_dict = attribute_link_instance.to_dict()
# create an instance of AttributeLink from a dict
attribute_link_from_dict = AttributeLink.from_dict(attribute_link_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


