# AttributeBool


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | **bool** |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_bool import AttributeBool

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeBool from a JSON string
attribute_bool_instance = AttributeBool.from_json(json)
# print the JSON string representation of the object
print(AttributeBool.to_json())

# convert the object into a dict
attribute_bool_dict = attribute_bool_instance.to_dict()
# create an instance of AttributeBool from a dict
attribute_bool_from_dict = AttributeBool.from_dict(attribute_bool_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


