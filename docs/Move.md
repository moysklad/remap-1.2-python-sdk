# Move

Перемещение

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Перемещения | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Перемещения | [optional] 
**code** | **str** | Код Перемещения | [optional] 
**external_code** | **str** | Внешний код Перемещения | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Перемещения | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Перемещения | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Перемещения | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**sum** | **float** | Сумма Перемещения в копейках | [optional] [readonly] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**source_store** | [**Store**](Store.md) | Метаданные склада, с которого совершается перемещение | [optional] 
**target_store** | [**Store**](Store.md) | Метаданные склада, на который совершается перемещение | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Перемещения | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**positions** | [**MovePositionList**](MovePositionList.md) |  | [optional] 
**overhead** | [**Overhead**](Overhead.md) |  | [optional] 
**internal_order** | [**InternalOrder**](InternalOrder.md) | Внутренний заказ, с которым связано Перемещение | [optional] 
**customer_order** | [**CustomerOrder**](CustomerOrder.md) | Заказ покупателя, с которым связано Перемещение | [optional] 
**demand** | [**Demand**](Demand.md) | Отгрузка, связанная с Перемещением | [optional] [readonly] 
**supply** | [**Supply**](Supply.md) | Приемка, связанная с Перемещением | [optional] [readonly] 
**production_tasks** | [**List[ProductionTask]**](ProductionTask.md) | Связанные производственные задания | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.move import Move

# TODO update the JSON string below
json = "{}"
# create an instance of Move from a JSON string
move_instance = Move.from_json(json)
# print the JSON string representation of the object
print(Move.to_json())

# convert the object into a dict
move_dict = move_instance.to_dict()
# create an instance of Move from a dict
move_from_dict = Move.from_dict(move_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


