# Payroll

Начисление зарплаты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Начисления зарплаты | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**description** | **str** | Описание Начисления зарплаты | [optional] 
**end_payroll_period** | **str** | Окончание расчётного периода, за который начисляется зарплата. Разница начала и окончания расчётного периода должна быть кратна 24 часам; секунды игнорируются.  | [optional] 
**external_code** | **str** | Внешний код Начисления зарплаты | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов (максимальное количество файлов — 100) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Наименование Начисления зарплаты | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**positions** | [**PayrollPositionList**](PayrollPositionList.md) |  | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**start_payroll_period** | **str** | Начало расчётного периода, за который начисляется зарплата. Разница начала и окончания расчётного периода должна быть кратна 24 часам; секунды игнорируются.  | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Начисления зарплаты | [optional] 
**sum** | **float** | Сумма Начисления зарплаты в копейках | [optional] [readonly] 
**sync_id** | **str** | ID синхронизации. После заполнения недоступен для изменения | [optional] 
**updated** | **str** | Момент последнего обновления Начисления зарплаты | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.payroll import Payroll

# TODO update the JSON string below
json = "{}"
# create an instance of Payroll from a JSON string
payroll_instance = Payroll.from_json(json)
# print the JSON string representation of the object
print(Payroll.to_json())

# convert the object into a dict
payroll_dict = payroll_instance.to_dict()
# create an instance of Payroll from a dict
payroll_from_dict = Payroll.from_dict(payroll_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


