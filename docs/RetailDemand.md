# RetailDemand

Розничная продажа

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Розничной продажи | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Розничной продажи | [optional] 
**code** | **str** | Код Розничной продажи | [optional] 
**external_code** | **str** | Внешний код Розничной продажи | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Розничной продажи | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Розничной продажи | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Розничной продажи | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] [readonly] 
**sum** | **float** | Сумма Розничной продажи в копейках | [optional] [readonly] 
**payed_sum** | **float** | Сумма входящих платежей по Розничной продаже | [optional] [readonly] 
**cash_sum** | **float** | Оплачено наличными | [optional] 
**no_cash_sum** | **float** | Оплачено картой | [optional] 
**qr_sum** | **float** | Оплачено по QR-коду | [optional] 
**prepayment_cash_sum** | **float** | Предоплата наличными | [optional] 
**prepayment_no_cash_sum** | **float** | Предоплата картой | [optional] 
**prepayment_qr_sum** | **float** | Предоплата по QR-коду | [optional] 
**advance_payment_sum** | **float** | Оплачено из аванса | [optional] 
**check_number** | **int** | Номер чека | [optional] 
**check_sum** | **float** | Сумма чека | [optional] 
**document_number** | **int** | Номер документа | [optional] 
**session_number** | **int** | Номер сессии | [optional] 
**tax_system** | **str** | Код системы налогообложения. Известные значения описаны в TaxSystem | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Розничной продажи | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] 
**store** | [**Store**](Store.md) |  | [optional] 
**retail_store** | [**RetailStore**](RetailStore.md) |  | [optional] 
**retail_shift** | [**RetailShift**](RetailShift.md) |  | [optional] 
**customer_order** | [**CustomerOrder**](CustomerOrder.md) | Метаданные заказа покупателя | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива файлов | [optional] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**positions** | [**RetailDemandPositionList**](RetailDemandPositionList.md) |  | [optional] 
**gift_cards** | [**List[RetailDemandGiftCard]**](RetailDemandGiftCard.md) | Коллекция подарочных сертификатов, используемых при оплате продажи | [optional] 
**cheque** | [**RetailDemandCheque**](RetailDemandCheque.md) | Фискальные данные продажи | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_demand import RetailDemand

# TODO update the JSON string below
json = "{}"
# create an instance of RetailDemand from a JSON string
retail_demand_instance = RetailDemand.from_json(json)
# print the JSON string representation of the object
print(RetailDemand.to_json())

# convert the object into a dict
retail_demand_dict = retail_demand_instance.to_dict()
# create an instance of RetailDemand from a dict
retail_demand_from_dict = RetailDemand.from_dict(retail_demand_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


