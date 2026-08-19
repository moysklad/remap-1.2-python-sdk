# TaskNoteList

Список комментариев к Задаче

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[TaskNote]**](TaskNote.md) | Массив комментариев к Задаче | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.task_note_list import TaskNoteList

# TODO update the JSON string below
json = "{}"
# create an instance of TaskNoteList from a JSON string
task_note_list_instance = TaskNoteList.from_json(json)
# print the JSON string representation of the object
print(TaskNoteList.to_json())

# convert the object into a dict
task_note_list_dict = task_note_list_instance.to_dict()
# create an instance of TaskNoteList from a dict
task_note_list_from_dict = TaskNoteList.from_dict(task_note_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


