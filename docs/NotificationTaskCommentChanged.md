# NotificationTaskCommentChanged

Уведомление об изменении комментария к задаче

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**diff** | [**NotificationTaskCommentDiff**](NotificationTaskCommentDiff.md) |  | [optional] 
**note_content** | **str** | Содержимое комментария | [optional] 
**performed_by** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**task** | [**NotificationTask**](NotificationTask.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task_comment_changed import NotificationTaskCommentChanged

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTaskCommentChanged from a JSON string
notification_task_comment_changed_instance = NotificationTaskCommentChanged.from_json(json)
# print the JSON string representation of the object
print(NotificationTaskCommentChanged.to_json())

# convert the object into a dict
notification_task_comment_changed_dict = notification_task_comment_changed_instance.to_dict()
# create an instance of NotificationTaskCommentChanged from a dict
notification_task_comment_changed_from_dict = NotificationTaskCommentChanged.from_dict(notification_task_comment_changed_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


