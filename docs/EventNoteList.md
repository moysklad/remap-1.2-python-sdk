# EventNoteList

Список Событий документа

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[EventNote]**](EventNote.md) | Массив Событий документа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.event_note_list import EventNoteList

# TODO update the JSON string below
json = "{}"
# create an instance of EventNoteList from a JSON string
event_note_list_instance = EventNoteList.from_json(json)
# print the JSON string representation of the object
print(EventNoteList.to_json())

# convert the object into a dict
event_note_list_dict = event_note_list_instance.to_dict()
# create an instance of EventNoteList from a dict
event_note_list_from_dict = EventNoteList.from_dict(event_note_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


