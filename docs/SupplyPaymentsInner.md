# SupplyPaymentsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Входящего платежа | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Входящего платежа | [optional] 
**code** | **str** | Код Входящего платежа | [optional] 
**external_code** | **str** | Внешний код Входящего платежа | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Входящего платежа | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Входящего платежа | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Входящего платежа | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента | [optional] 
**expense_item** | [**ExpenseItem**](ExpenseItem.md) | Метаданные статьи расходов | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива файлов | [optional] 
**no_closing_docs** | **bool** | Признак \&quot;Без закрывающих документов\&quot; | [optional] 
**payment_purpose** | **str** | Назначение платежа | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**sales_channel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж | [optional] 
**shared** | **bool** | Общий доступ | [optional] [readonly] 
**state** | [**State**](State.md) | Метаданные статуса Входящего платежа | [optional] 
**sum** | **float** | Сумма Входящего платежа в установленной валюте | [optional] [readonly] 
**vat_sum** | **float** | Сумма НДС | [optional] 
**facture_in** | [**FactureIn**](FactureIn.md) | Счет-фактура полученный, с которым связан этот платеж | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**operations** | [**List[FinanceInOperationAbstract]**](FinanceInOperationAbstract.md) | Связанные операции. Допустимые типы по &#x60;meta.type&#x60;: customerorder, purchasereturn, demand, invoiceout, commissionreportin, retailshift.  | [optional] 
**incoming_number** | **str** | Входящий номер | [optional] 
**incoming_date** | **str** | Входящая дата | [optional] 
**facture_out** | [**FactureOut**](FactureOut.md) | Счет-фактура выданный, с которым связан этот платеж | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.supply_payments_inner import SupplyPaymentsInner

# TODO update the JSON string below
json = "{}"
# create an instance of SupplyPaymentsInner from a JSON string
supply_payments_inner_instance = SupplyPaymentsInner.from_json(json)
# print the JSON string representation of the object
print(SupplyPaymentsInner.to_json())

# convert the object into a dict
supply_payments_inner_dict = supply_payments_inner_instance.to_dict()
# create an instance of SupplyPaymentsInner from a dict
supply_payments_inner_from_dict = SupplyPaymentsInner.from_dict(supply_payments_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


