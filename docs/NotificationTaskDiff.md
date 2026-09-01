# NotificationTaskDiff

Измененные поля задачи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | [**NotificationDiffValue**](NotificationDiffValue.md) |  | [optional] 
**deadline** | [**NotificationDiffValue**](NotificationDiffValue.md) |  | [optional] 
**agent_link** | [**NotificationDiffValue**](NotificationDiffValue.md) |  | [optional] 
**document_link** | [**NotificationDiffValue**](NotificationDiffValue.md) |  | [optional] 
**assignee** | [**NotificationDiffValue**](NotificationDiffValue.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task_diff import NotificationTaskDiff

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTaskDiff from a JSON string
notification_task_diff_instance = NotificationTaskDiff.from_json(json)
# print the JSON string representation of the object
print(NotificationTaskDiff.to_json())

# convert the object into a dict
notification_task_diff_dict = notification_task_diff_instance.to_dict()
# create an instance of NotificationTaskDiff from a dict
notification_task_diff_from_dict = NotificationTaskDiff.from_dict(notification_task_diff_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


