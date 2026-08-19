# ScriptPermissions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**view** | **str** | Смотреть. Известные значения описаны в ScriptPermissionValue. | [optional] 
**create** | **str** | Создавать. Известные значения описаны в ScriptPermissionValue. | [optional] 
**update** | **str** | Редактировать. Известные значения описаны в ScriptPermissionValue. | [optional] 
**delete** | **str** | Удалять. Известные значения описаны в ScriptPermissionValue. | [optional] 
**done** | **str** | Выполнять. Известные значения описаны в ScriptPermissionValue. | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.script_permissions import ScriptPermissions

# TODO update the JSON string below
json = "{}"
# create an instance of ScriptPermissions from a JSON string
script_permissions_instance = ScriptPermissions.from_json(json)
# print the JSON string representation of the object
print(ScriptPermissions.to_json())

# convert the object into a dict
script_permissions_dict = script_permissions_instance.to_dict()
# create an instance of ScriptPermissions from a dict
script_permissions_from_dict = ScriptPermissions.from_dict(script_permissions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


