# TaskNotes

Метаданные комментариев к задаче

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[TaskNote]**](TaskNote.md) | Массив комментариев к задаче | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.task_notes import TaskNotes

# TODO update the JSON string below
json = "{}"
# create an instance of TaskNotes from a JSON string
task_notes_instance = TaskNotes.from_json(json)
# print the JSON string representation of the object
print(TaskNotes.to_json())

# convert the object into a dict
task_notes_dict = task_notes_instance.to_dict()
# create an instance of TaskNotes from a dict
task_notes_from_dict = TaskNotes.from_dict(task_notes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


