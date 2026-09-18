# ScriptPermissions

Права на задачи. NO для view и done допустимо, только если остальные права равны NO. Если view отличается от NO, поле done обязательно и должно совпадать с view. Известные значения описаны в ScriptPermissionValue. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**view** | **str** | Смотреть. Допустимые значения — NO, AUTHOR_OR_ASSIGNEE, ALL. Известные значения описаны в ScriptPermissionValue. | [optional] 
**create** | **str** | Создавать. Допустимые значения — NO, ALL. Область действия не шире view; поле может отсутствовать. Известные значения описаны в ScriptPermissionValue. | [optional] 
**update** | **str** | Редактировать. Допустимые значения — NO, AUTHOR, AUTHOR_OR_ASSIGNEE, ALL. Область действия не шире view; поле может отсутствовать. Известные значения описаны в ScriptPermissionValue. | [optional] 
**delete** | **str** | Удалять. Допустимые значения — NO, AUTHOR, AUTHOR_OR_ASSIGNEE, ALL. Область действия не шире update; поле может отсутствовать. Известные значения описаны в ScriptPermissionValue. | [optional] 
**done** | **str** | Выполнять. Допустимые значения — NO, ASSIGNEE, AUTHOR_OR_ASSIGNEE, ALL. Область действия не шире view; при view, отличном от NO, обязательно и совпадает с view. Известные значения описаны в ScriptPermissionValue. | [optional] 

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


