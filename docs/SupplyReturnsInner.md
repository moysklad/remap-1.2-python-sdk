# SupplyReturnsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Возврата предоплаты | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Возврата предоплаты | [optional] 
**code** | **str** | Код Возврата предоплаты | [optional] 
**external_code** | **str** | Внешний код Возврата предоплаты | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Возврата предоплаты | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Возврата предоплаты | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Возврата предоплаты | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] 
**sum** | **float** | Сумма Возврата предоплаты в копейках | [optional] [readonly] 
**payed_sum** | **float** | Сумма входящих платежей по Возврату поставщику | [optional] [readonly] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные Контрагента или юрлица | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] 
**store** | [**Store**](Store.md) |  | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Возврата предоплаты | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**rate** | [**CurrencyRate**](.md) |  | [optional] 
**positions** | [**PrepaymentReturnPositionList**](PrepaymentReturnPositionList.md) |  | [optional] 
**sales_channel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж | [optional] 
**demand** | [**Demand**](Demand.md) | Отгрузка, по которой произошел возврат | [optional] 
**losses** | [**List[Loss]**](Loss.md) | Массив ссылок на связанные списания | [optional] 
**payments** | [**List[RetailShiftPaymentsInner]**](RetailShiftPaymentsInner.md) | Массив ссылок на связанные платежи | [optional] 
**facture_out** | [**FactureOut**](FactureOut.md) | Счет-фактура выданный, с которым связан этот возврат | [optional] 
**supply** | [**Supply**](Supply.md) | Приемка, по которой произошел возврат | [optional] 
**facture_in** | [**FactureIn**](FactureIn.md) | Счет-фактура полученный, с которым связан этот возврат | [optional] 
**cash_sum** | **float** | Оплачено наличными | [optional] 
**no_cash_sum** | **float** | Оплачено картой | [optional] 
**qr_sum** | **float** | Оплачено по QR-коду | [optional] 
**prepayment** | [**Prepayment**](Prepayment.md) |  | [optional] 
**retail_shift** | [**RetailShift**](RetailShift.md) |  | [optional] 
**retail_store** | [**RetailStore**](RetailStore.md) |  | [optional] 
**tax_system** | **str** | Код системы налогообложения. Известные значения описаны в TaxSystem | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.supply_returns_inner import SupplyReturnsInner

# TODO update the JSON string below
json = "{}"
# create an instance of SupplyReturnsInner from a JSON string
supply_returns_inner_instance = SupplyReturnsInner.from_json(json)
# print the JSON string representation of the object
print(SupplyReturnsInner.to_json())

# convert the object into a dict
supply_returns_inner_dict = supply_returns_inner_instance.to_dict()
# create an instance of SupplyReturnsInner from a dict
supply_returns_inner_from_dict = SupplyReturnsInner.from_dict(supply_returns_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


