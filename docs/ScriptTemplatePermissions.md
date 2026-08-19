# ScriptTemplatePermissions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**view** | **str** | Смотреть. Известные значения описаны в PermissionValue. | [optional] 
**create** | **str** | Создавать. Известные значения описаны в PermissionValue. | [optional] 
**update** | **str** | Редактировать. Известные значения описаны в PermissionValue. | [optional] 
**delete** | **str** | Удалять. Известные значения описаны в PermissionValue. | [optional] 
**activate** | **str** | Выполнять. Известные значения описаны в PermissionValue. | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.script_template_permissions import ScriptTemplatePermissions

# TODO update the JSON string below
json = "{}"
# create an instance of ScriptTemplatePermissions from a JSON string
script_template_permissions_instance = ScriptTemplatePermissions.from_json(json)
# print the JSON string representation of the object
print(ScriptTemplatePermissions.to_json())

# convert the object into a dict
script_template_permissions_dict = script_template_permissions_instance.to_dict()
# create an instance of ScriptTemplatePermissions from a dict
script_template_permissions_from_dict = ScriptTemplatePermissions.from_dict(script_template_permissions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


