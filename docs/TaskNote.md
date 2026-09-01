# TaskNote

Комментарий к Задаче

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID комментария к Задаче | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**author** | [**Employee**](Employee.md) |  | [optional] 
**author_application** | [**Application**](Application.md) |  | [optional] 
**moment** | **str** | Момент создания комментария | [optional] [readonly] 
**text** | **str** | Текст комментария | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.task_note import TaskNote

# TODO update the JSON string below
json = "{}"
# create an instance of TaskNote from a JSON string
task_note_instance = TaskNote.from_json(json)
# print the JSON string representation of the object
print(TaskNote.to_json())

# convert the object into a dict
task_note_dict = task_note_instance.to_dict()
# create an instance of TaskNote from a dict
task_note_from_dict = TaskNote.from_dict(task_note_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


