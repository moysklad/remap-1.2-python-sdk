# NotificationTaskCompleted

Уведомление о выполнении задачи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**performed_by** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**task** | [**NotificationTask**](NotificationTask.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task_completed import NotificationTaskCompleted

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTaskCompleted from a JSON string
notification_task_completed_instance = NotificationTaskCompleted.from_json(json)
# print the JSON string representation of the object
print(NotificationTaskCompleted.to_json())

# convert the object into a dict
notification_task_completed_dict = notification_task_completed_instance.to_dict()
# create an instance of NotificationTaskCompleted from a dict
notification_task_completed_from_dict = NotificationTaskCompleted.from_dict(notification_task_completed_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


