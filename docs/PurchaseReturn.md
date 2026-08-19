# PurchaseReturn

Возврат поставщику

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID возврата поставщику | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Возврата поставщику | [optional] 
**code** | **str** | Код Возврата поставщику | [optional] 
**external_code** | **str** | Внешний код Возврата поставщику | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Возврата поставщику | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Возврата поставщику | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Возврата поставщику | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] [readonly] 
**sum** | **float** | Сумма Возврата поставщику в копейках | [optional] [readonly] 
**payed_sum** | **float** | Сумма входящих платежей по Возврату поставщику | [optional] [readonly] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] 
**store** | [**Store**](Store.md) |  | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Возврата поставщику | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**rate** | [**CurrencyRate**](.md) | Валюта документа. Если значение курса валюты не указано, используется курс из справочника валют.  | [optional] 
**positions** | [**PurchaseReturnPositionList**](PurchaseReturnPositionList.md) | Позиции Возврата поставщику | [optional] 
**supply** | [**Supply**](Supply.md) | Приемка, по которой произошел возврат | [optional] 
**facture_out** | [**FactureOut**](FactureOut.md) | Счет-фактура выданный, с которым связан этот возврат | [optional] 
**facture_in** | [**FactureIn**](FactureIn.md) | Счет-фактура полученный, с которым связан этот возврат | [optional] 
**payments** | [**List[RetailShiftPaymentsInner]**](RetailShiftPaymentsInner.md) | Массив ссылок на связанные платежи | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.purchase_return import PurchaseReturn

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseReturn from a JSON string
purchase_return_instance = PurchaseReturn.from_json(json)
# print the JSON string representation of the object
print(PurchaseReturn.to_json())

# convert the object into a dict
purchase_return_dict = purchase_return_instance.to_dict()
# create an instance of PurchaseReturn from a dict
purchase_return_from_dict = PurchaseReturn.from_dict(purchase_return_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


