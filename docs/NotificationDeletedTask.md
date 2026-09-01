# NotificationDeletedTask

Краткое представление удаленной задачи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Наименование задачи | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_deleted_task import NotificationDeletedTask

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationDeletedTask from a JSON string
notification_deleted_task_instance = NotificationDeletedTask.from_json(json)
# print the JSON string representation of the object
print(NotificationDeletedTask.to_json())

# convert the object into a dict
notification_deleted_task_dict = notification_deleted_task_instance.to_dict()
# create an instance of NotificationDeletedTask from a dict
notification_deleted_task_from_dict = NotificationDeletedTask.from_dict(notification_deleted_task_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


