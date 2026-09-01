# NotificationTaskDeleted

Уведомление об удалении задачи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**performed_by** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**task** | [**NotificationDeletedTask**](NotificationDeletedTask.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task_deleted import NotificationTaskDeleted

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTaskDeleted from a JSON string
notification_task_deleted_instance = NotificationTaskDeleted.from_json(json)
# print the JSON string representation of the object
print(NotificationTaskDeleted.to_json())

# convert the object into a dict
notification_task_deleted_dict = notification_task_deleted_instance.to_dict()
# create an instance of NotificationTaskDeleted from a dict
notification_task_deleted_from_dict = NotificationTaskDeleted.from_dict(notification_task_deleted_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


