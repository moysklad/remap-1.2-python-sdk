# CashIn

Приходный ордер

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Приходного ордера | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**name** | **str** | Наименование Приходного ордера | [optional] 
**code** | **str** | Код Приходного ордера | [optional] 
**external_code** | **str** | Внешний код Приходного ордера | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Приходного ордера | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Приходного ордера | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Приходного ордера | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива файлов | [optional] 
**payment_purpose** | **str** | Основание | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**sales_channel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж | [optional] 
**shared** | **bool** | Общий доступ | [optional] [readonly] 
**state** | [**State**](State.md) | Метаданные статуса Приходного ордера | [optional] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица | [optional] 
**sum** | **float** | Сумма Приходного ордера в установленной валюте | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] 
**facture_out** | [**FactureOut**](FactureOut.md) | Счет-фактура выданный, с которым связан этот платеж | [optional] 
**operations** | [**List[FinanceInOperationAbstract]**](FinanceInOperationAbstract.md) | Связанные операции. Допустимые типы по &#x60;meta.type&#x60;: customerorder, purchasereturn, demand, invoiceout, commissionreportin, retailshift.  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.cash_in import CashIn

# TODO update the JSON string below
json = "{}"
# create an instance of CashIn from a JSON string
cash_in_instance = CashIn.from_json(json)
# print the JSON string representation of the object
print(CashIn.to_json())

# convert the object into a dict
cash_in_dict = cash_in_instance.to_dict()
# create an instance of CashIn from a dict
cash_in_from_dict = CashIn.from_dict(cash_in_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


