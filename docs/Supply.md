# Supply

Приемка

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Приемки | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Приемки | [optional] 
**code** | **str** | Код Приемки | [optional] 
**external_code** | **str** | Внешний код Приемки | [optional] 
**sync_id** | **str** | ID синхронизации. После заполнения недоступен для изменения | [optional] 
**description** | **str** | Комментарий Приемки | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Приемки | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Приемки | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**incoming_date** | **str** | Входящая дата | [optional] 
**incoming_number** | **str** | Входящий номер | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] [readonly] 
**sum** | **float** | Сумма Приемки в копейках | [optional] [readonly] 
**payed_sum** | **float** | Сумма входящих платежей по Приемке | [optional] [readonly] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] 
**store** | [**Store**](Store.md) | Метаданные склада | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Приемки | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов (максимальное количество файлов — 100) | [optional] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**overhead** | [**Overhead**](Overhead.md) |  | [optional] 
**positions** | [**SupplyPositionList**](SupplyPositionList.md) |  | [optional] 
**purchase_order** | [**PurchaseOrder**](PurchaseOrder.md) | Заказ поставщику, с которым связана Приемка  | [optional] 
**facture_in** | [**FactureIn**](FactureIn.md) | Счет-фактура полученный, с которым связана эта Приемка | [optional] 
**invoices_in** | [**List[InvoiceIn]**](InvoiceIn.md) | Массив ссылок на связанные счета поставщиков | [optional] 
**payments** | [**List[SupplyPaymentsInner]**](SupplyPaymentsInner.md) | Массив ссылок на связанные платежи | [optional] 
**production_task** | [**ProductionTask**](ProductionTask.md) | Связанное производственное задание | [optional] 
**returns** | [**List[SupplyReturnsInner]**](SupplyReturnsInner.md) | Массив ссылок на связанные возвраты  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.supply import Supply

# TODO update the JSON string below
json = "{}"
# create an instance of Supply from a JSON string
supply_instance = Supply.from_json(json)
# print the JSON string representation of the object
print(Supply.to_json())

# convert the object into a dict
supply_dict = supply_instance.to_dict()
# create an instance of Supply from a dict
supply_from_dict = Supply.from_dict(supply_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


