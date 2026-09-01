# NotificationTaskChanged

Уведомление об изменении задачи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**diff** | [**NotificationTaskDiff**](NotificationTaskDiff.md) |  | [optional] 
**performed_by** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**task** | [**NotificationTask**](NotificationTask.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task_changed import NotificationTaskChanged

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTaskChanged from a JSON string
notification_task_changed_instance = NotificationTaskChanged.from_json(json)
# print the JSON string representation of the object
print(NotificationTaskChanged.to_json())

# convert the object into a dict
notification_task_changed_dict = notification_task_changed_instance.to_dict()
# create an instance of NotificationTaskChanged from a dict
notification_task_changed_from_dict = NotificationTaskChanged.from_dict(notification_task_changed_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


