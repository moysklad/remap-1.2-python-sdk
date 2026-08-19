# TaskNoteFileList

Файлы комментария к Задаче

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[TaskNoteFile]**](TaskNoteFile.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.task_note_file_list import TaskNoteFileList

# TODO update the JSON string below
json = "{}"
# create an instance of TaskNoteFileList from a JSON string
task_note_file_list_instance = TaskNoteFileList.from_json(json)
# print the JSON string representation of the object
print(TaskNoteFileList.to_json())

# convert the object into a dict
task_note_file_list_dict = task_note_file_list_instance.to_dict()
# create an instance of TaskNoteFileList from a dict
task_note_file_list_from_dict = TaskNoteFileList.from_dict(task_note_file_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


