# NotificationTaskUnassigned

Уведомление о снятии задачи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**performed_by** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**task** | [**NotificationTask**](NotificationTask.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task_unassigned import NotificationTaskUnassigned

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTaskUnassigned from a JSON string
notification_task_unassigned_instance = NotificationTaskUnassigned.from_json(json)
# print the JSON string representation of the object
print(NotificationTaskUnassigned.to_json())

# convert the object into a dict
notification_task_unassigned_dict = notification_task_unassigned_instance.to_dict()
# create an instance of NotificationTaskUnassigned from a dict
notification_task_unassigned_from_dict = NotificationTaskUnassigned.from_dict(notification_task_unassigned_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


