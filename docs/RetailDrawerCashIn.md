# RetailDrawerCashIn

Внесение денег

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Внесения денег | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**agent** | [**Employee**](Employee.md) |  | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Внесения денег | [optional] [readonly] 
**description** | **str** | Комментарий Внесения денег | [optional] 
**external_code** | **str** | Внешний код Внесения денег | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива файлов | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Наименование Внесения денег | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**rate** | [**CurrencyRate**](CurrencyRate.md) |  | [optional] 
**retail_shift** | [**RetailShift**](RetailShift.md) |  | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Внесения денег | [optional] 
**sum** | **float** | Сумма Внесения денег в копейках | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**updated** | **str** | Момент последнего обновления Внесения денег | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_drawer_cash_in import RetailDrawerCashIn

# TODO update the JSON string below
json = "{}"
# create an instance of RetailDrawerCashIn from a JSON string
retail_drawer_cash_in_instance = RetailDrawerCashIn.from_json(json)
# print the JSON string representation of the object
print(RetailDrawerCashIn.to_json())

# convert the object into a dict
retail_drawer_cash_in_dict = retail_drawer_cash_in_instance.to_dict()
# create an instance of RetailDrawerCashIn from a dict
retail_drawer_cash_in_from_dict = RetailDrawerCashIn.from_dict(retail_drawer_cash_in_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


