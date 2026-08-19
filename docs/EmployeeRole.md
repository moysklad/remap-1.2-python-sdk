# EmployeeRole

Роль сотрудника

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**permissions** | [**EmployeeRolePermissions**](EmployeeRolePermissions.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.employee_role import EmployeeRole

# TODO update the JSON string below
json = "{}"
# create an instance of EmployeeRole from a JSON string
employee_role_instance = EmployeeRole.from_json(json)
# print the JSON string representation of the object
print(EmployeeRole.to_json())

# convert the object into a dict
employee_role_dict = employee_role_instance.to_dict()
# create an instance of EmployeeRole from a dict
employee_role_from_dict = EmployeeRole.from_dict(employee_role_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


