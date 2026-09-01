# NotificationTaskCommentDiff

Изменение текста комментария к задаче

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**note_content** | [**NotificationDiffValue**](NotificationDiffValue.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_task_comment_diff import NotificationTaskCommentDiff

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTaskCommentDiff from a JSON string
notification_task_comment_diff_instance = NotificationTaskCommentDiff.from_json(json)
# print the JSON string representation of the object
print(NotificationTaskCommentDiff.to_json())

# convert the object into a dict
notification_task_comment_diff_dict = notification_task_comment_diff_instance.to_dict()
# create an instance of NotificationTaskCommentDiff from a dict
notification_task_comment_diff_from_dict = NotificationTaskCommentDiff.from_dict(notification_task_comment_diff_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


