# AttributeAbstract


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | ID дополнительного поля | [optional] 
**name** | **str** | Наименование дополнительного поля | [optional] 
**type** | **str** |  | 
**meta** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_abstract import AttributeAbstract

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeAbstract from a JSON string
attribute_abstract_instance = AttributeAbstract.from_json(json)
# print the JSON string representation of the object
print(AttributeAbstract.to_json())

# convert the object into a dict
attribute_abstract_dict = attribute_abstract_instance.to_dict()
# create an instance of AttributeAbstract from a dict
attribute_abstract_from_dict = AttributeAbstract.from_dict(attribute_abstract_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


