# AttributeString


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_string import AttributeString

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeString from a JSON string
attribute_string_instance = AttributeString.from_json(json)
# print the JSON string representation of the object
print(AttributeString.to_json())

# convert the object into a dict
attribute_string_dict = attribute_string_instance.to_dict()
# create an instance of AttributeString from a dict
attribute_string_from_dict = AttributeString.from_dict(attribute_string_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


