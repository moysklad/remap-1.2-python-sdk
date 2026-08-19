# AttributeEmployeeEntity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | [**Employee**](Employee.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_employee_entity import AttributeEmployeeEntity

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeEmployeeEntity from a JSON string
attribute_employee_entity_instance = AttributeEmployeeEntity.from_json(json)
# print the JSON string representation of the object
print(AttributeEmployeeEntity.to_json())

# convert the object into a dict
attribute_employee_entity_dict = attribute_employee_entity_instance.to_dict()
# create an instance of AttributeEmployeeEntity from a dict
attribute_employee_entity_from_dict = AttributeEmployeeEntity.from_dict(attribute_employee_entity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


