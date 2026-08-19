# CustomRole

Пользовательская роль

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID пользовательской роли | [optional] [readonly] 
**name** | **str** | Наименование пользовательской роли | [optional] 
**permissions** | [**EmployeeRolePermissions**](EmployeeRolePermissions.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.custom_role import CustomRole

# TODO update the JSON string below
json = "{}"
# create an instance of CustomRole from a JSON string
custom_role_instance = CustomRole.from_json(json)
# print the JSON string representation of the object
print(CustomRole.to_json())

# convert the object into a dict
custom_role_dict = custom_role_instance.to_dict()
# create an instance of CustomRole from a dict
custom_role_from_dict = CustomRole.from_dict(custom_role_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


