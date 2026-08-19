# Project

Проект

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID проекта | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**archived** | **bool** | Добавлен ли Проект в архив | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция доп. полей | [optional] 
**code** | **str** | Код Проекта | [optional] 
**description** | **str** | Описание Проекта | [optional] 
**external_code** | **str** | Внешний код Проекта | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**name** | **str** | Наименование Проекта | [optional] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**updated** | **str** | Момент последнего обновления сущности | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.project import Project

# TODO update the JSON string below
json = "{}"
# create an instance of Project from a JSON string
project_instance = Project.from_json(json)
# print the JSON string representation of the object
print(Project.to_json())

# convert the object into a dict
project_dict = project_instance.to_dict()
# create an instance of Project from a dict
project_from_dict = Project.from_dict(project_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


