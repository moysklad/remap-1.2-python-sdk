# NotificationExportCompleted

Уведомление о завершении экспорта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_document_name** | **str** | Имя экспортированного документа | [optional] 
**error_message** | **str** | Сообщение об ошибке | [optional] 
**message** | **str** | Сообщение о завершении экспорта | [optional] 
**task_state** | **str** | Статус завершения. Известные значения описаны в NotificationTaskState | [optional] 
**task_type** | **str** | Тип экспорта. Известные значения описаны в NotificationExportType | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_export_completed import NotificationExportCompleted

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationExportCompleted from a JSON string
notification_export_completed_instance = NotificationExportCompleted.from_json(json)
# print the JSON string representation of the object
print(NotificationExportCompleted.to_json())

# convert the object into a dict
notification_export_completed_dict = notification_export_completed_instance.to_dict()
# create an instance of NotificationExportCompleted from a dict
notification_export_completed_from_dict = NotificationExportCompleted.from_dict(notification_export_completed_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


