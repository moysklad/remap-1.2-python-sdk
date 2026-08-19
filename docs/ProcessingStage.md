# ProcessingStage

Этап производства

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Этапа производства | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**updated** | **str** | Момент последнего обновления Этапа производства | [optional] [readonly] 
**name** | **str** | Наименование Этапа производства | [optional] 
**description** | **str** | Комментарий Этапа производства | [optional] 
**external_code** | **str** | Внешний код Этапа производства | [optional] 
**archived** | **bool** | Добавлен ли Этап производства в архив | [optional] 
**all_performers** | **bool** | Признак доступности назначения на этап любого сотрудника | [optional] 
**distribution_required** | **bool** | Признак видимости заданий для исполнителей в веб-приложении МойСклад Производство | [optional] 
**performers** | [**List[Agent]**](Agent.md) | Метаданные возможных исполнителей | [optional] 
**material_store** | [**Store**](Store.md) | Метаданные склада материалов | [optional] [readonly] 
**standard_hour_cost** | **float** | Стоимость нормо-часа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_stage import ProcessingStage

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingStage from a JSON string
processing_stage_instance = ProcessingStage.from_json(json)
# print the JSON string representation of the object
print(ProcessingStage.to_json())

# convert the object into a dict
processing_stage_dict = processing_stage_instance.to_dict()
# create an instance of ProcessingStage from a dict
processing_stage_from_dict = ProcessingStage.from_dict(processing_stage_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


