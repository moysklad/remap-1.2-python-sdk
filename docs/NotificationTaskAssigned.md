# NotificationTaskAssigned

Уведомление о назначении задачи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**performed_by** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**task** | [**NotificationTask**](NotificationTask.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task_assigned import NotificationTaskAssigned

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTaskAssigned from a JSON string
notification_task_assigned_instance = NotificationTaskAssigned.from_json(json)
# print the JSON string representation of the object
print(NotificationTaskAssigned.to_json())

# convert the object into a dict
notification_task_assigned_dict = notification_task_assigned_instance.to_dict()
# create an instance of NotificationTaskAssigned from a dict
notification_task_assigned_from_dict = NotificationTaskAssigned.from_dict(notification_task_assigned_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


