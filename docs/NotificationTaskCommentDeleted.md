# NotificationTaskCommentDeleted

Уведомление об удалении комментария к задаче

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**note_content** | **str** | Содержимое удаленного комментария | [optional] 
**performed_by** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**task** | [**NotificationTask**](NotificationTask.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task_comment_deleted import NotificationTaskCommentDeleted

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTaskCommentDeleted from a JSON string
notification_task_comment_deleted_instance = NotificationTaskCommentDeleted.from_json(json)
# print the JSON string representation of the object
print(NotificationTaskCommentDeleted.to_json())

# convert the object into a dict
notification_task_comment_deleted_dict = notification_task_comment_deleted_instance.to_dict()
# create an instance of NotificationTaskCommentDeleted from a dict
notification_task_comment_deleted_from_dict = NotificationTaskCommentDeleted.from_dict(notification_task_comment_deleted_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


