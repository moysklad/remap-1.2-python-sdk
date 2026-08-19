# Loss

Списание

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Списания | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**code** | **str** | Код Списания | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Списания | [optional] [readonly] 
**description** | **str** | Комментарий Списания | [optional] 
**expense_item** | [**ExpenseItem**](ExpenseItem.md) | Метаданные Статьи расходов | [optional] [readonly] 
**external_code** | **str** | Внешний код Списания | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов (Максимальное количество файлов - 100) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Наименование Списания | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**positions** | [**LossPositionList**](LossPositionList.md) |  | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**rate** | [**CurrencyRate**](.md) | Валюта документа.  Если значение курса валюты не указано, используется курс из справочника валют.  | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Списания | [optional] 
**store** | [**Store**](Store.md) |  | [optional] 
**sum** | **float** | Сумма Списания в копейках | [optional] [readonly] 
**sync_id** | **str** | ID синхронизации | [optional] 
**updated** | **str** | Момент последнего обновления Списания | [optional] [readonly] 
**sales_return** | [**SalesReturn**](SalesReturn.md) | Связанный со Списанием возврат покупателя | [optional] 
**inventory** | [**Inventory**](Inventory.md) | Связанная со Списанием инвентаризация | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.loss import Loss

# TODO update the JSON string below
json = "{}"
# create an instance of Loss from a JSON string
loss_instance = Loss.from_json(json)
# print the JSON string representation of the object
print(Loss.to_json())

# convert the object into a dict
loss_dict = loss_instance.to_dict()
# create an instance of Loss from a dict
loss_from_dict = Loss.from_dict(loss_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


