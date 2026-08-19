# AttributeMetaField

Поле meta в доп. полях

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_meta_field import AttributeMetaField

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeMetaField from a JSON string
attribute_meta_field_instance = AttributeMetaField.from_json(json)
# print the JSON string representation of the object
print(AttributeMetaField.to_json())

# convert the object into a dict
attribute_meta_field_dict = attribute_meta_field_instance.to_dict()
# create an instance of AttributeMetaField from a dict
attribute_meta_field_from_dict = AttributeMetaField.from_dict(attribute_meta_field_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


