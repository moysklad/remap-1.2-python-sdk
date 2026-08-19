# PurchaseOrder

Заказ поставщику

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Заказа поставщику | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Заказа поставщику | [optional] 
**code** | **str** | Код Заказа поставщику | [optional] 
**external_code** | **str** | Внешний код Заказа поставщику | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Заказа поставщику | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Заказа поставщику | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Заказа поставщику | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**delivery_planned_moment** | **str** | Планируемая дата отгрузки | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] [readonly] 
**sum** | **float** | Сумма Заказа поставщику в установленной валюте | [optional] [readonly] 
**payed_sum** | **float** | Сумма входящих платежей по Заказу | [optional] [readonly] 
**shipped_sum** | **float** | Сумма принятого | [optional] [readonly] 
**invoiced_sum** | **float** | Сумма счетов поставщику | [optional] [readonly] 
**wait_sum** | **float** | Сумма товаров в пути | [optional] [readonly] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] 
**store** | [**Store**](Store.md) | Метаданные склада | [optional] 
**state** | [**State**](State.md) | Метаданные статуса заказа | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**rate** | [**PurchaseOrderRate**](PurchaseOrderRate.md) |  | [optional] 
**positions** | [**PurchaseOrderPositionList**](PurchaseOrderPositionList.md) |  | [optional] 
**internal_order** | [**InternalOrder**](InternalOrder.md) | Внутренний заказ, связанный с заказом поставщику | [optional] 
**customer_orders** | [**List[CustomerOrder]**](CustomerOrder.md) | Массив ссылок на связанные заказы покупателей | [optional] 
**invoices_in** | [**List[InvoiceIn]**](InvoiceIn.md) | Массив ссылок на связанные счета поставщиков | [optional] 
**supplies** | [**List[Supply]**](Supply.md) | Массив ссылок на связанные приемки | [optional] 
**payments** | [**List[SalesReturnPaymentsInner]**](SalesReturnPaymentsInner.md) | Массив ссылок на связанные платежи | [optional] 
**production_tasks** | [**List[ProductionTask]**](ProductionTask.md) | Массив ссылок на связанные производственные задания | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.purchase_order import PurchaseOrder

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseOrder from a JSON string
purchase_order_instance = PurchaseOrder.from_json(json)
# print the JSON string representation of the object
print(PurchaseOrder.to_json())

# convert the object into a dict
purchase_order_dict = purchase_order_instance.to_dict()
# create an instance of PurchaseOrder from a dict
purchase_order_from_dict = PurchaseOrder.from_dict(purchase_order_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


