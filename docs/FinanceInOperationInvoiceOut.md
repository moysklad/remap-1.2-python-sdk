# FinanceInOperationInvoiceOut

Счет покупателю + linkedSum

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Счета покупателя | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Счета покупателя | [optional] 
**code** | **str** | Код Счета покупателя | [optional] 
**external_code** | **str** | Внешний код Счета покупателя | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Счета покупателя | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Счета покупателя | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Счета покупателя | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**payment_planned_moment** | **str** | Планируемая дата оплаты | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] [readonly] 
**sum** | **float** | Сумма Счета в установленной валюте | [optional] [readonly] 
**payed_sum** | **float** | Сумма входящих платежей по Счету покупателя | [optional] [readonly] 
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
**positions** | [**InvoiceOutPositionList**](InvoiceOutPositionList.md) |  | [optional] 
**sales_channel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж | [optional] 
**customer_order** | [**CustomerOrder**](CustomerOrder.md) | Заказ покупателя, с которым связан Счет покупателю | [optional] 
**demands** | [**List[Demand]**](Demand.md) | Массив ссылок на связанные отгрузки | [optional] 
**payments** | [**List[RetailShiftPaymentsInner]**](RetailShiftPaymentsInner.md) | Массив ссылок на связанные операции | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.finance_in_operation_invoice_out import FinanceInOperationInvoiceOut

# TODO update the JSON string below
json = "{}"
# create an instance of FinanceInOperationInvoiceOut from a JSON string
finance_in_operation_invoice_out_instance = FinanceInOperationInvoiceOut.from_json(json)
# print the JSON string representation of the object
print(FinanceInOperationInvoiceOut.to_json())

# convert the object into a dict
finance_in_operation_invoice_out_dict = finance_in_operation_invoice_out_instance.to_dict()
# create an instance of FinanceInOperationInvoiceOut from a dict
finance_in_operation_invoice_out_from_dict = FinanceInOperationInvoiceOut.from_dict(finance_in_operation_invoice_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


