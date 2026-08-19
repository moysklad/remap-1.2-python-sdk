# TaskNoteFile

Файл комментария к Задаче

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID файла | [optional] [readonly] 
**title** | **str** | Название файла | [optional] 
**filename** | **str** | Имя файла | [optional] 
**content** | **str** | Файл, закодированный в Base64 | [optional] 
**size** | **int** | Размер файла в байтах | [optional] [readonly] 
**created** | **str** | Время создания объекта | [optional] [readonly] 
**created_by** | [**Employee**](Employee.md) |  | [optional] 
**tiny** | [**Meta**](Meta.md) |  | [optional] 
**miniature** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.task_note_file import TaskNoteFile

# TODO update the JSON string below
json = "{}"
# create an instance of TaskNoteFile from a JSON string
task_note_file_instance = TaskNoteFile.from_json(json)
# print the JSON string representation of the object
print(TaskNoteFile.to_json())

# convert the object into a dict
task_note_file_dict = task_note_file_instance.to_dict()
# create an instance of TaskNoteFile from a dict
task_note_file_from_dict = TaskNoteFile.from_dict(task_note_file_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


