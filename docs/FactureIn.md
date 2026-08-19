# FactureIn

Счет-фактура полученный (facturein)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Счета-фактуры полученного | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**code** | **str** | Код Счета-фактуры полученного | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Счета-фактуры полученного | [optional] [readonly] 
**description** | **str** | Комментарий Счета-фактуры полученного | [optional] 
**external_code** | **str** | Внешний код Счета-фактуры полученного | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива файлов | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Наименование Счета-фактуры полученного | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**rate** | [**CurrencyRate**](.md) | Валюта документа. Если значение курса валюты не указано, используется курс из справочника валют.  | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Счета-фактуры полученного | [optional] 
**sum** | **float** | Сумма Счета-фактуры полученного в установленной валюте | [optional] [readonly] 
**sync_id** | **str** | ID синхронизации | [optional] 
**updated** | **str** | Момент последнего обновления Счета-фактуры полученного | [optional] [readonly] 
**supplies** | [**List[Supply]**](Supply.md) | Массив ссылок на связанные приемки | [optional] 
**payments** | [**List[PaymentOut]**](PaymentOut.md) | Массив ссылок на связанные исходящие платежи | [optional] 
**incoming_number** | **str** | Входящий номер | [optional] 
**incoming_date** | **str** | Входящая дата | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.facture_in import FactureIn

# TODO update the JSON string below
json = "{}"
# create an instance of FactureIn from a JSON string
facture_in_instance = FactureIn.from_json(json)
# print the JSON string representation of the object
print(FactureIn.to_json())

# convert the object into a dict
facture_in_dict = facture_in_instance.to_dict()
# create an instance of FactureIn from a dict
facture_in_from_dict = FactureIn.from_dict(facture_in_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


