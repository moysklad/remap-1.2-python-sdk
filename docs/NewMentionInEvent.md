# NewMentionInEvent

Уведомление о новом упоминании в ленте событий

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**operation** | [**NotificationNamedEntity**](NotificationNamedEntity.md) | Объект, в ленте которого добавлено событие с упоминанием | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.new_mention_in_event import NewMentionInEvent

# TODO update the JSON string below
json = "{}"
# create an instance of NewMentionInEvent from a JSON string
new_mention_in_event_instance = NewMentionInEvent.from_json(json)
# print the JSON string representation of the object
print(NewMentionInEvent.to_json())

# convert the object into a dict
new_mention_in_event_dict = new_mention_in_event_instance.to_dict()
# create an instance of NewMentionInEvent from a dict
new_mention_in_event_from_dict = NewMentionInEvent.from_dict(new_mention_in_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


