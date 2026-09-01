# AppChangePermissions

Уведомление об устаревших правах доступа в решении

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID уведомления | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**created** | **str** | Дата и время формирования уведомления | [optional] [readonly] 
**read** | **bool** | Признак того, было ли уведомление прочитано | [optional] 
**title** | **str** | Краткий текст уведомления | [optional] [readonly] 
**description** | **str** | Описание уведомления | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.app_change_permissions import AppChangePermissions

# TODO update the JSON string below
json = "{}"
# create an instance of AppChangePermissions from a JSON string
app_change_permissions_instance = AppChangePermissions.from_json(json)
# print the JSON string representation of the object
print(AppChangePermissions.to_json())

# convert the object into a dict
app_change_permissions_dict = app_change_permissions_instance.to_dict()
# create an instance of AppChangePermissions from a dict
app_change_permissions_from_dict = AppChangePermissions.from_dict(app_change_permissions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


