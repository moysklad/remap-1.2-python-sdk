# InvoiceIn

Счет поставщика

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Счета поставщика | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Счета поставщика | [optional] 
**code** | **str** | Код Счета поставщика | [optional] 
**external_code** | **str** | Внешний код Счета поставщика | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Счета поставщика | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Счета поставщика | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Счета поставщика | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**payment_planned_moment** | **str** | Планируемая дата оплаты | [optional] 
**incoming_date** | **str** | Входящая дата | [optional] 
**incoming_number** | **str** | Входящий номер | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] [readonly] 
**sum** | **float** | Сумма Счета в установленной валюте | [optional] [readonly] 
**payed_sum** | **float** | Сумма входящих платежей по Счету поставщика | [optional] [readonly] 
**shipped_sum** | **float** | Сумма отгруженного | [optional] [readonly] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] 
**store** | [**Store**](Store.md) | Метаданные склада | [optional] 
**state** | [**State**](State.md) | Метаданные статуса счета | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**positions** | [**InvoiceInPositionList**](InvoiceInPositionList.md) |  | [optional] 
**purchase_order** | [**PurchaseOrder**](PurchaseOrder.md) | Заказ поставщику, с которым связан Счет поставщика | [optional] 
**supplies** | [**List[Supply]**](Supply.md) | Массив ссылок на связанные приемки | [optional] 
**payments** | [**List[SalesReturnPaymentsInner]**](SalesReturnPaymentsInner.md) | Массив ссылок на связанные операции | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.invoice_in import InvoiceIn

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceIn from a JSON string
invoice_in_instance = InvoiceIn.from_json(json)
# print the JSON string representation of the object
print(InvoiceIn.to_json())

# convert the object into a dict
invoice_in_dict = invoice_in_instance.to_dict()
# create an instance of InvoiceIn from a dict
invoice_in_from_dict = InvoiceIn.from_dict(invoice_in_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


