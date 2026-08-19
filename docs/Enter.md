# Enter

Оприходование

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Оприходования | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**code** | **str** | Код Оприходования | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Оприходования | [optional] [readonly] 
**description** | **str** | Комментарий Оприходования | [optional] 
**external_code** | **str** | Внешний код Оприходования | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Номер Оприходования | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**overhead** | [**Overhead**](Overhead.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**positions** | [**EnterPositionList**](EnterPositionList.md) | Метаданные позиций Оприходования | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**rate** | [**CurrencyRate**](.md) | Валюта документа. Если значение курса валюты не указано, используется курс из справочника валют.  | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Оприходования | [optional] 
**store** | [**Store**](Store.md) |  | [optional] 
**sum** | **float** | Сумма Оприходования в копейках | [optional] [readonly] 
**sync_id** | **str** | ID синхронизации | [optional] 
**updated** | **str** | Момент последнего обновления Оприходования | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.enter import Enter

# TODO update the JSON string below
json = "{}"
# create an instance of Enter from a JSON string
enter_instance = Enter.from_json(json)
# print the JSON string representation of the object
print(Enter.to_json())

# convert the object into a dict
enter_dict = enter_instance.to_dict()
# create an instance of Enter from a dict
enter_from_dict = Enter.from_dict(enter_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


