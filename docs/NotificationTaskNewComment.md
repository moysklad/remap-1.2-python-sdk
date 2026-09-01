# NotificationTaskNewComment

Уведомление о новом комментарии к задаче

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**note_content** | **str** | Содержимое комментария | [optional] 
**performed_by** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**task** | [**NotificationTask**](NotificationTask.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task_new_comment import NotificationTaskNewComment

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTaskNewComment from a JSON string
notification_task_new_comment_instance = NotificationTaskNewComment.from_json(json)
# print the JSON string representation of the object
print(NotificationTaskNewComment.to_json())

# convert the object into a dict
notification_task_new_comment_dict = notification_task_new_comment_instance.to_dict()
# create an instance of NotificationTaskNewComment from a dict
notification_task_new_comment_from_dict = NotificationTaskNewComment.from_dict(notification_task_new_comment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


