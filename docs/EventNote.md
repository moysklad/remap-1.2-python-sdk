# EventNote

Событие в Ленте документа

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID События | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**created** | **str** | Момент создания События | [optional] [readonly] 
**description** | **str** | Текст События | [optional] 
**author** | [**Employee**](Employee.md) |  | [optional] 
**author_application** | [**Application**](Application.md) | Метаданные Решения - создателя События | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.event_note import EventNote

# TODO update the JSON string below
json = "{}"
# create an instance of EventNote from a JSON string
event_note_instance = EventNote.from_json(json)
# print the JSON string representation of the object
print(EventNote.to_json())

# convert the object into a dict
event_note_dict = event_note_instance.to_dict()
# create an instance of EventNote from a dict
event_note_from_dict = EventNote.from_dict(event_note_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


