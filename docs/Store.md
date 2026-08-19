# Store

Склад

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Склада | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**updated** | **str** | Момент последнего обновления | [optional] [readonly] 
**name** | **str** | Наименование Склада | [optional] 
**description** | **str** | Комментарий к Складу | [optional] 
**code** | **str** | Код Склада | [optional] 
**external_code** | **str** | Внешний код Склада | [optional] 
**archived** | **bool** | Добавлен ли в архив | [optional] 
**address** | **str** | Адрес склада | [optional] 
**address_full** | [**Address**](Address.md) | Адрес с детализацией | [optional] 
**path_name** | **str** | Группа Склада | [optional] [readonly] 
**parent** | [**Store**](Store.md) | Метаданные родительского склада (Группы) | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Дополнительные поля | [optional] 
**zones** | [**StoreZoneList**](StoreZoneList.md) | Зоны склада | [optional] 
**slots** | [**StoreSlotList**](StoreSlotList.md) | Ячейки склада | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.store import Store

# TODO update the JSON string below
json = "{}"
# create an instance of Store from a JSON string
store_instance = Store.from_json(json)
# print the JSON string representation of the object
print(Store.to_json())

# convert the object into a dict
store_dict = store_instance.to_dict()
# create an instance of Store from a dict
store_from_dict = Store.from_dict(store_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


