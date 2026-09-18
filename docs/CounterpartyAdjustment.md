# CounterpartyAdjustment

Корректировка взаиморасчетов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Корректировки взаиморасчетов | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента или сотрудника | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Корректировки взаиморасчетов | [optional] [readonly] 
**description** | **str** | Комментарий Корректировки взаиморасчетов | [optional] 
**external_code** | **str** | Внешний код Корректировки взаиморасчетов | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов (максимум 100) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Наименование Корректировки взаиморасчетов | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**sum** | **float** | Сумма Корректировки взаиморасчетов в копейках | [optional] 
**updated** | **str** | Момент последнего обновления Корректировки взаиморасчетов | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.counterparty_adjustment import CounterpartyAdjustment

# TODO update the JSON string below
json = "{}"
# create an instance of CounterpartyAdjustment from a JSON string
counterparty_adjustment_instance = CounterpartyAdjustment.from_json(json)
# print the JSON string representation of the object
print(CounterpartyAdjustment.to_json())

# convert the object into a dict
counterparty_adjustment_dict = counterparty_adjustment_instance.to_dict()
# create an instance of CounterpartyAdjustment from a dict
counterparty_adjustment_from_dict = CounterpartyAdjustment.from_dict(counterparty_adjustment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


