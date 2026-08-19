# SalesReturn

Возврат покупателя

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Возврата покупателя | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Возврата покупателя | [optional] 
**code** | **str** | Код Возврата покупателя | [optional] 
**external_code** | **str** | Внешний код Возврата покупателя | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Возврата покупателя | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Возврата покупателя | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Возврата покупателя | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] 
**sum** | **float** | Сумма Возврата покупателя в копейках | [optional] [readonly] 
**payed_sum** | **float** | Сумма исходящих платежей по Возврату покупателя | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные Контрагента или юрлица | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] 
**store** | [**Store**](Store.md) | Метаданные склада | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Возврата покупателя | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**rate** | [**CurrencyRate**](.md) | Валюта документа.  Если значение курса валюты не указано, используется курс из справочника валют.  | [optional] 
**positions** | [**SalesReturnPositionList**](SalesReturnPositionList.md) |  | [optional] 
**sales_channel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж | [optional] 
**demand** | [**Demand**](Demand.md) | Отгрузка, по которой произошел возврат | [optional] 
**losses** | [**List[Loss]**](Loss.md) | Массив ссылок на связанные списания | [optional] 
**payments** | [**List[SalesReturnPaymentsInner]**](SalesReturnPaymentsInner.md) | Массив ссылок на связанные платежи | [optional] 
**facture_out** | [**FactureOut**](FactureOut.md) | Счет-фактура выданный, с которым связан этот возврат | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.sales_return import SalesReturn

# TODO update the JSON string below
json = "{}"
# create an instance of SalesReturn from a JSON string
sales_return_instance = SalesReturn.from_json(json)
# print the JSON string representation of the object
print(SalesReturn.to_json())

# convert the object into a dict
sales_return_dict = sales_return_instance.to_dict()
# create an instance of SalesReturn from a dict
sales_return_from_dict = SalesReturn.from_dict(sales_return_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


