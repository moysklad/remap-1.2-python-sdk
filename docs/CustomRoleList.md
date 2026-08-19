# CustomRoleList

Список пользовательских ролей

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[CustomRole]**](CustomRole.md) | Массив пользовательских ролей | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.custom_role_list import CustomRoleList

# TODO update the JSON string below
json = "{}"
# create an instance of CustomRoleList from a JSON string
custom_role_list_instance = CustomRoleList.from_json(json)
# print the JSON string representation of the object
print(CustomRoleList.to_json())

# convert the object into a dict
custom_role_list_dict = custom_role_list_instance.to_dict()
# create an instance of CustomRoleList from a dict
custom_role_list_from_dict = CustomRoleList.from_dict(custom_role_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


