# AttributeDateTime


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_date_time import AttributeDateTime

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeDateTime from a JSON string
attribute_date_time_instance = AttributeDateTime.from_json(json)
# print the JSON string representation of the object
print(AttributeDateTime.to_json())

# convert the object into a dict
attribute_date_time_dict = attribute_date_time_instance.to_dict()
# create an instance of AttributeDateTime from a dict
attribute_date_time_from_dict = AttributeDateTime.from_dict(attribute_date_time_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


