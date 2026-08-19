# ProcessingPlanFolder

Группа техкарт

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Группы техкарт | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Группы техкарт | [optional] 
**code** | **str** | Код Группы техкарт | [optional] 
**external_code** | **str** | Внешний код Группы техкарт | [optional] 
**description** | **str** | Описание Группы техкарт | [optional] 
**archived** | **bool** | Добавлена ли Группа техкарт в архив | [optional] 
**path_name** | **str** | Наименование группы техкарт, в которую входит данная группа (иерархия) | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**updated** | **str** | Момент последнего обновления сущности | [optional] [readonly] 
**group** | [**Group**](Group.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (сотрудника) | [optional] 
**processingplanfolder** | [**ProcessingPlanFolder**](ProcessingPlanFolder.md) | Родительская Группа техкарт. Для смены иерархии и поля pathName обновите эту ссылку | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_plan_folder import ProcessingPlanFolder

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingPlanFolder from a JSON string
processing_plan_folder_instance = ProcessingPlanFolder.from_json(json)
# print the JSON string representation of the object
print(ProcessingPlanFolder.to_json())

# convert the object into a dict
processing_plan_folder_dict = processing_plan_folder_instance.to_dict()
# create an instance of ProcessingPlanFolder from a dict
processing_plan_folder_from_dict = ProcessingPlanFolder.from_dict(processing_plan_folder_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


