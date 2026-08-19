# FinanceInOperationDemand

Отгрузка + linkedSum

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Отгрузки | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Отгрузки | [optional] 
**code** | **str** | Код Отгрузки | [optional] 
**external_code** | **str** | Внешний код Отгрузки | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Отгрузки | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Отгрузки | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Отгрузки | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включён ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] [readonly] 
**sum** | **float** | Сумма Отгрузки в копейках | [optional] [readonly] 
**payed_sum** | **float** | Сумма входящих платежей по Отгрузке | [optional] [readonly] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] 
**store** | [**Store**](Store.md) | Метаданные склада | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Отгрузки | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива файлов | [optional] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**positions** | [**DemandPositionList**](DemandPositionList.md) |  | [optional] 
**sales_channel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж | [optional] 
**shipment_address** | **str** | Адрес доставки Отгрузки (строка). Для удаления адреса передайте пустую строку. Не поддерживается значение &#x60;null&#x60; для сброса — см. документацию по адресу доставки.  | [optional] 
**shipment_address_full** | [**Address**](Address.md) | Адрес доставки Отгрузки с детализацией по отдельным полям | [optional] 
**overhead** | [**Overhead**](Overhead.md) |  | [optional] 
**customer_order** | [**CustomerOrder**](CustomerOrder.md) | Заказ покупателя, с которым связана Отгрузка | [optional] 
**facture_out** | [**FactureOut**](FactureOut.md) | Счёт-фактура выданный, с которым связана Отгрузка | [optional] 
**returns** | [**List[SalesReturn]**](SalesReturn.md) | Связанные возвраты | [optional] 
**payments** | [**List[RetailShiftPaymentsInner]**](RetailShiftPaymentsInner.md) | Связанные платежи | [optional] 
**production_tasks** | [**List[ProductionTask]**](ProductionTask.md) | Связанные производственные задания | [optional] 
**invoices_out** | [**List[InvoiceOut]**](InvoiceOut.md) | Связанные счета покупателям | [optional] 
**cargo_name** | **str** | Наименование груза | [optional] 
**carrier** | [**Agent**](Agent.md) | Перевозчик (контрагент или юрлицо) | [optional] 
**consignee** | [**Agent**](Agent.md) | Грузополучатель (контрагент или юрлицо) | [optional] 
**good_pack_quantity** | **int** | Всего мест | [optional] 
**shipping_instructions** | **str** | Указания грузоотправителя | [optional] 
**state_contract_id** | **str** | Идентификатор государственного контракта, договора (соглашения) | [optional] 
**transport_facility** | **str** | Транспортное средство | [optional] 
**transport_facility_number** | **str** | Номер автомобиля | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.finance_in_operation_demand import FinanceInOperationDemand

# TODO update the JSON string below
json = "{}"
# create an instance of FinanceInOperationDemand from a JSON string
finance_in_operation_demand_instance = FinanceInOperationDemand.from_json(json)
# print the JSON string representation of the object
print(FinanceInOperationDemand.to_json())

# convert the object into a dict
finance_in_operation_demand_dict = finance_in_operation_demand_instance.to_dict()
# create an instance of FinanceInOperationDemand from a dict
finance_in_operation_demand_from_dict = FinanceInOperationDemand.from_dict(finance_in_operation_demand_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


