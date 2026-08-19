# FinanceInOperationCustomerOrder

Заказ покупателя + linkedSum

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Заказа покупателя | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Заказа покупателя | [optional] 
**code** | **str** | Код Заказа покупателя | [optional] 
**external_code** | **str** | Внешний код Заказа покупателя | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Заказа покупателя | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Заказа покупателя | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Заказа покупателя | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**delivery_planned_moment** | **str** | Планируемая дата приёмки | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] [readonly] 
**sum** | **float** | Сумма Заказа в установленной валюте | [optional] [readonly] 
**payed_sum** | **float** | Сумма входящих платежей по Заказу | [optional] [readonly] 
**shipped_sum** | **float** | Сумма отгруженного | [optional] [readonly] 
**reserved_sum** | **float** | Сумма товаров в резерве | [optional] [readonly] 
**invoiced_sum** | **float** | Сумма счетов покупателю | [optional] [readonly] 
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
**tax_system** | **str** | Код системы налогообложения. Известные значения описаны в TaxSystem | [optional] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**positions** | [**CustomerOrderPositionList**](CustomerOrderPositionList.md) |  | [optional] 
**sales_channel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж | [optional] 
**shipment_address** | **str** | Адрес доставки Заказа покупателя | [optional] 
**shipment_address_full** | [**Address**](Address.md) | Адрес доставки Заказа покупателя с детализацией по отдельным полям | [optional] 
**invoices_out** | [**List[InvoiceOut]**](InvoiceOut.md) | Массив ссылок на связанные счета покупателям | [optional] 
**demands** | [**List[Demand]**](Demand.md) | Массив ссылок на связанные отгрузки | [optional] 
**payments** | [**List[RetailShiftPaymentsInner]**](RetailShiftPaymentsInner.md) | Массив ссылок на связанные платежи | [optional] 
**prepayments** | [**List[Prepayment]**](Prepayment.md) | Массив ссылок на связанные предоплаты | [optional] 
**purchase_orders** | [**List[PurchaseOrder]**](PurchaseOrder.md) | Массив ссылок на связанные заказы поставщикам | [optional] 
**moves** | [**List[Move]**](Move.md) | Массив ссылок на связанные перемещения | [optional] 
**production_tasks** | [**List[ProductionTask]**](ProductionTask.md) | Массив ссылок на связанные производственные задания | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.finance_in_operation_customer_order import FinanceInOperationCustomerOrder

# TODO update the JSON string below
json = "{}"
# create an instance of FinanceInOperationCustomerOrder from a JSON string
finance_in_operation_customer_order_instance = FinanceInOperationCustomerOrder.from_json(json)
# print the JSON string representation of the object
print(FinanceInOperationCustomerOrder.to_json())

# convert the object into a dict
finance_in_operation_customer_order_dict = finance_in_operation_customer_order_instance.to_dict()
# create an instance of FinanceInOperationCustomerOrder from a dict
finance_in_operation_customer_order_from_dict = FinanceInOperationCustomerOrder.from_dict(finance_in_operation_customer_order_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


