# AttributeFile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**download** | **object** |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_file import AttributeFile

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeFile from a JSON string
attribute_file_instance = AttributeFile.from_json(json)
# print the JSON string representation of the object
print(AttributeFile.to_json())

# convert the object into a dict
attribute_file_dict = attribute_file_instance.to_dict()
# create an instance of AttributeFile from a dict
attribute_file_from_dict = AttributeFile.from_dict(attribute_file_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


