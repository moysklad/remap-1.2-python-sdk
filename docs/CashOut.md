# CashOut

Расходный ордер

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Расходного ордера | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Расходного ордера | [optional] 
**code** | **str** | Код Расходного ордера | [optional] 
**external_code** | **str** | Внешний код Расходного ордера | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Расходного ордера | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Расходного ордера | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Расходного ордера | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица | [optional] 
**expense_item** | [**ExpenseItem**](ExpenseItem.md) | Метаданные статьи расхода | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива файлов | [optional] 
**no_closing_docs** | **bool** | Признак \&quot;Без закрывающих документов\&quot; | [optional] 
**payment_purpose** | **str** | Основание | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**sales_channel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж | [optional] 
**shared** | **bool** | Общий доступ | [optional] [readonly] 
**state** | [**State**](State.md) | Метаданные статуса Расходного ордера | [optional] 
**sum** | **float** | Сумма расходного ордера в установленной валюте | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] 
**facture_in** | [**FactureIn**](FactureIn.md) | Счет-фактура полученный, с которым связан этот платеж | [optional] 
**operations** | [**List[FinanceOutOperationAbstract]**](FinanceOutOperationAbstract.md) | Связанные операции: полное тело документа плюс &#x60;linkedSum&#x60;. Допустимые типы по &#x60;meta.type&#x60;: salesreturn, supply, invoicein, purchaseorder, commissionreportout  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.cash_out import CashOut

# TODO update the JSON string below
json = "{}"
# create an instance of CashOut from a JSON string
cash_out_instance = CashOut.from_json(json)
# print the JSON string representation of the object
print(CashOut.to_json())

# convert the object into a dict
cash_out_dict = cash_out_instance.to_dict()
# create an instance of CashOut from a dict
cash_out_from_dict = CashOut.from_dict(cash_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


