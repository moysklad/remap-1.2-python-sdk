# NotificationTask

Краткое представление задачи в уведомлении

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID объекта | [optional] 
**name** | **str** | Наименование объекта | [optional] 
**deadline** | **str** | Планируемая дата завершения задачи | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task import NotificationTask

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTask from a JSON string
notification_task_instance = NotificationTask.from_json(json)
# print the JSON string representation of the object
print(NotificationTask.to_json())

# convert the object into a dict
notification_task_dict = notification_task_instance.to_dict()
# create an instance of NotificationTask from a dict
notification_task_from_dict = NotificationTask.from_dict(notification_task_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


