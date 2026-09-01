# NewEventInEventFeed

Уведомление о новом событии в отслеживаемом объекте

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**entity** | [**NotificationNamedEntity**](NotificationNamedEntity.md) | Объект, в ленте которого добавлено событие | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.new_event_in_event_feed import NewEventInEventFeed

# TODO update the JSON string below
json = "{}"
# create an instance of NewEventInEventFeed from a JSON string
new_event_in_event_feed_instance = NewEventInEventFeed.from_json(json)
# print the JSON string representation of the object
print(NewEventInEventFeed.to_json())

# convert the object into a dict
new_event_in_event_feed_dict = new_event_in_event_feed_instance.to_dict()
# create an instance of NewEventInEventFeed from a dict
new_event_in_event_feed_from_dict = NewEventInEventFeed.from_dict(new_event_in_event_feed_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


