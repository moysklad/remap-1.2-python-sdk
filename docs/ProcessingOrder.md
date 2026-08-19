# ProcessingOrder

Заказ на производство

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID заказа на производство | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование заказа на производство | [optional] 
**code** | **str** | Код заказа на производство | [optional] 
**external_code** | **str** | Внешний код заказа на производство | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий заказа на производство | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления заказа на производство | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления заказа на производство | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**delivery_planned_moment** | **str** | Планируемая дата производства | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] [readonly] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**store** | [**Store**](Store.md) |  | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Заказа на производство | [optional] 
**processing_plan** | [**ProcessingPlan**](ProcessingPlan.md) |  | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**positions** | [**ProcessingOrderPositionList**](.md) | Позиции Заказа на производство | [optional] 
**quantity** | **float** | Объем производства | [optional] 
**processings** | [**List[Processing]**](Processing.md) | Массив ссылок на связанные техоперации | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_order import ProcessingOrder

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingOrder from a JSON string
processing_order_instance = ProcessingOrder.from_json(json)
# print the JSON string representation of the object
print(ProcessingOrder.to_json())

# convert the object into a dict
processing_order_dict = processing_order_instance.to_dict()
# create an instance of ProcessingOrder from a dict
processing_order_from_dict = ProcessingOrder.from_dict(processing_order_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


