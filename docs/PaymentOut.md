# PaymentOut

Исходящий платеж

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Исходящего платежа | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Исходящего платежа | [optional] 
**code** | **str** | Код Исходящего платежа | [optional] 
**external_code** | **str** | Внешний код Исходящего платежа | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Исходящего платежа | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Исходящего платежа | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Исходящего платежа | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента, сотрудника или юрлица | [optional] 
**expense_item** | [**ExpenseItem**](ExpenseItem.md) | Метаданные статьи расходов | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива файлов | [optional] 
**no_closing_docs** | **bool** | Признак \&quot;Без закрывающих документов\&quot; | [optional] 
**payment_purpose** | **str** | Назначение платежа | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**sales_channel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж | [optional] 
**shared** | **bool** | Общий доступ | [optional] [readonly] 
**state** | [**State**](State.md) | Метаданные статуса Исходящего платежа | [optional] 
**sum** | **float** | Сумма Исходящего платежа в установленной валюте | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] 
**facture_in** | [**FactureIn**](FactureIn.md) | Счет-фактура полученный, с которым связан этот платеж | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента или юрлица | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**operations** | [**List[FinanceOutOperationAbstract]**](FinanceOutOperationAbstract.md) | Связанные операции: полное тело документа плюс &#x60;linkedSum&#x60;. Допустимые типы по &#x60;meta.type&#x60;: salesreturn, supply, invoicein, purchaseorder, commissionreportout  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.payment_out import PaymentOut

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentOut from a JSON string
payment_out_instance = PaymentOut.from_json(json)
# print the JSON string representation of the object
print(PaymentOut.to_json())

# convert the object into a dict
payment_out_dict = payment_out_instance.to_dict()
# create an instance of PaymentOut from a dict
payment_out_from_dict = PaymentOut.from_dict(payment_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


