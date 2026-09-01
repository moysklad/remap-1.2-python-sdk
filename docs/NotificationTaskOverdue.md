# NotificationTaskOverdue

Уведомление о просроченной задаче

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**task** | [**NotificationTask**](NotificationTask.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task_overdue import NotificationTaskOverdue

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTaskOverdue from a JSON string
notification_task_overdue_instance = NotificationTaskOverdue.from_json(json)
# print the JSON string representation of the object
print(NotificationTaskOverdue.to_json())

# convert the object into a dict
notification_task_overdue_dict = notification_task_overdue_instance.to_dict()
# create an instance of NotificationTaskOverdue from a dict
notification_task_overdue_from_dict = NotificationTaskOverdue.from_dict(notification_task_overdue_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


