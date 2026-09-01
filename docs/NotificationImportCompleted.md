# NotificationImportCompleted

Уведомление о завершении импорта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_document_name** | **str** | Имя созданного документа | [optional] 
**error_message** | **str** | Сообщение об ошибке | [optional] 
**message** | **str** | Сообщение о завершении импорта | [optional] 
**task_state** | **str** | Статус завершения. Известные значения описаны в NotificationTaskState | [optional] 
**task_type** | **str** | Тип импорта. Известные значения описаны в NotificationImportType | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_import_completed import NotificationImportCompleted

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationImportCompleted from a JSON string
notification_import_completed_instance = NotificationImportCompleted.from_json(json)
# print the JSON string representation of the object
print(NotificationImportCompleted.to_json())

# convert the object into a dict
notification_import_completed_dict = notification_import_completed_instance.to_dict()
# create an instance of NotificationImportCompleted from a dict
notification_import_completed_from_dict = NotificationImportCompleted.from_dict(notification_import_completed_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


