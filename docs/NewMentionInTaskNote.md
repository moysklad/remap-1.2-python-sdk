# NewMentionInTaskNote

Уведомление о новом упоминании в комментарии задачи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**task** | [**NotificationNamedEntity**](NotificationNamedEntity.md) | Задача с комментарием, содержащим упоминание | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.new_mention_in_task_note import NewMentionInTaskNote

# TODO update the JSON string below
json = "{}"
# create an instance of NewMentionInTaskNote from a JSON string
new_mention_in_task_note_instance = NewMentionInTaskNote.from_json(json)
# print the JSON string representation of the object
print(NewMentionInTaskNote.to_json())

# convert the object into a dict
new_mention_in_task_note_dict = new_mention_in_task_note_instance.to_dict()
# create an instance of NewMentionInTaskNote from a dict
new_mention_in_task_note_from_dict = NewMentionInTaskNote.from_dict(new_mention_in_task_note_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


