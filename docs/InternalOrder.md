# InternalOrder

Внутренний заказ

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Внутреннего заказа | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Внутреннего заказа | [optional] 
**code** | **str** | Код Внутреннего заказа | [optional] 
**external_code** | **str** | Внешний код Внутреннего заказа | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Внутреннего заказа | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Внутреннего заказа | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Внутреннего заказа | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**delivery_planned_moment** | **str** | Планируемая дата приемки | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] [readonly] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] [readonly] 
**sum** | **float** | Сумма Внутреннего заказа в копейках | [optional] [readonly] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**store** | [**Store**](Store.md) | Метаданные склада | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Внутреннего заказа | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**positions** | [**InternalOrderPositionList**](InternalOrderPositionList.md) |  | [optional] 
**purchase_orders** | [**List[PurchaseOrder]**](PurchaseOrder.md) | Коллекция метаданных на связанные заказы поставщику | [optional] 
**production_tasks** | [**List[ProductionTask]**](ProductionTask.md) | Массив ссылок на связанные производственные задания | [optional] 
**moves** | [**List[Move]**](Move.md) | Коллекция метаданных на связанные заказы перемещения | [optional] 
**processing_order** | [**ProcessingOrder**](ProcessingOrder.md) | Метаданные Заказа на производство | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.internal_order import InternalOrder

# TODO update the JSON string below
json = "{}"
# create an instance of InternalOrder from a JSON string
internal_order_instance = InternalOrder.from_json(json)
# print the JSON string representation of the object
print(InternalOrder.to_json())

# convert the object into a dict
internal_order_dict = internal_order_instance.to_dict()
# create an instance of InternalOrder from a dict
internal_order_from_dict = InternalOrder.from_dict(internal_order_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


