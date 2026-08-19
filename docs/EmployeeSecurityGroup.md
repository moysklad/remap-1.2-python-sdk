# EmployeeSecurityGroup

Метаданные Группы, а также ее идентификатор и имя

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID группы | [optional] 
**name** | **str** | Название группы | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.employee_security_group import EmployeeSecurityGroup

# TODO update the JSON string below
json = "{}"
# create an instance of EmployeeSecurityGroup from a JSON string
employee_security_group_instance = EmployeeSecurityGroup.from_json(json)
# print the JSON string representation of the object
print(EmployeeSecurityGroup.to_json())

# convert the object into a dict
employee_security_group_dict = employee_security_group_instance.to_dict()
# create an instance of EmployeeSecurityGroup from a dict
employee_security_group_from_dict = EmployeeSecurityGroup.from_dict(employee_security_group_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


