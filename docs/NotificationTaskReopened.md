# NotificationTaskReopened

Уведомление о повторном открытии задачи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**performed_by** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**task** | [**NotificationTask**](NotificationTask.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task_reopened import NotificationTaskReopened

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTaskReopened from a JSON string
notification_task_reopened_instance = NotificationTaskReopened.from_json(json)
# print the JSON string representation of the object
print(NotificationTaskReopened.to_json())

# convert the object into a dict
notification_task_reopened_dict = notification_task_reopened_instance.to_dict()
# create an instance of NotificationTaskReopened from a dict
notification_task_reopened_from_dict = NotificationTaskReopened.from_dict(notification_task_reopened_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


