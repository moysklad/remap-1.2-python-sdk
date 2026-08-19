# Task

Задача

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Задачи | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**agent** | [**Agent**](Agent.md) | Метаданные Контрагента или юрлица, связанного с задачей | [optional] 
**assignee** | [**Employee**](Employee.md) |  | [optional] 
**author** | [**Employee**](Employee.md) |  | [optional] 
**author_application** | [**Application**](Application.md) |  | [optional] 
**completed** | **str** | Время выполнения задачи | [optional] [readonly] 
**created** | **str** | Момент создания | [optional] [readonly] 
**description** | **str** | Текст задачи | [optional] 
**done** | **bool** | Отметка о выполнении задачи | [optional] 
**due_to_date** | **str** | Срок задачи | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**implementer** | [**Employee**](Employee.md) |  | [optional] 
**notes** | [**TaskNotes**](TaskNotes.md) |  | [optional] 
**operation** | [**DocumentMetadata**](DocumentMetadata.md) |  | [optional] 
**state** | [**State**](State.md) | Метаданные типа задачи | [optional] 
**updated** | **str** | Момент последнего обновления Задачи | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.task import Task

# TODO update the JSON string below
json = "{}"
# create an instance of Task from a JSON string
task_instance = Task.from_json(json)
# print the JSON string representation of the object
print(Task.to_json())

# convert the object into a dict
task_dict = task_instance.to_dict()
# create an instance of Task from a dict
task_from_dict = Task.from_dict(task_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


