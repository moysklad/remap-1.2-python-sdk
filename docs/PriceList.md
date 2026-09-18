# PriceList

Прайс-лист

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Прайс-листа | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**code** | **str** | Код Прайс-листа | [optional] 
**columns** | [**List[PriceListColumn]**](PriceListColumn.md) | Массив столбцов описания таблицы | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Прайс-листа | [optional] [readonly] 
**description** | **str** | Комментарий Прайс-листа | [optional] 
**external_code** | **str** | Внешний код Прайс-листа | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Наименование Прайс-листа | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**positions** | [**PriceListPositionList**](PriceListPositionList.md) | Метаданные позиций Прайс-листа | [optional] 
**price_type** | [**PriceType**](PriceType.md) | Объект типа цены | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Прайс-листа | [optional] 
**sync_id** | **str** | ID синхронизации. После заполнения недоступен для изменения | [optional] 
**updated** | **str** | Момент последнего обновления Прайс-листа | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.price_list import PriceList

# TODO update the JSON string below
json = "{}"
# create an instance of PriceList from a JSON string
price_list_instance = PriceList.from_json(json)
# print the JSON string representation of the object
print(PriceList.to_json())

# convert the object into a dict
price_list_dict = price_list_instance.to_dict()
# create an instance of PriceList from a dict
price_list_from_dict = PriceList.from_dict(price_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


