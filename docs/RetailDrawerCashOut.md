# RetailDrawerCashOut

Выплата денег

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Выплаты денег | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**agent** | [**Employee**](Employee.md) |  | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**code** | **str** | Код Выплаты денег | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Выплаты денег | [optional] [readonly] 
**description** | **str** | Комментарий Выплаты денег | [optional] 
**external_code** | **str** | Внешний код Выплаты денег | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива файлов | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Наименование Выплаты денег | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**retail_shift** | [**RetailShift**](RetailShift.md) |  | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Выплаты денег | [optional] 
**sum** | **float** | Сумма Выплаты денег в установленной валюте | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**updated** | **str** | Момент последнего обновления Выплаты денег | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_drawer_cash_out import RetailDrawerCashOut

# TODO update the JSON string below
json = "{}"
# create an instance of RetailDrawerCashOut from a JSON string
retail_drawer_cash_out_instance = RetailDrawerCashOut.from_json(json)
# print the JSON string representation of the object
print(RetailDrawerCashOut.to_json())

# convert the object into a dict
retail_drawer_cash_out_dict = retail_drawer_cash_out_instance.to_dict()
# create an instance of RetailDrawerCashOut from a dict
retail_drawer_cash_out_from_dict = RetailDrawerCashOut.from_dict(retail_drawer_cash_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


