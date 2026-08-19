# Uom

Единица измерения

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID единицы измерения | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование единицы измерения | [optional] 
**description** | **str** | Описание единицы измерения | [optional] 
**code** | **str** | Код единицы измерения | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**updated** | **str** | Момент последнего обновления сущности | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**external_code** | **str** | Внешний код единицы измерения | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.uom import Uom

# TODO update the JSON string below
json = "{}"
# create an instance of Uom from a JSON string
uom_instance = Uom.from_json(json)
# print the JSON string representation of the object
print(Uom.to_json())

# convert the object into a dict
uom_dict = uom_instance.to_dict()
# create an instance of Uom from a dict
uom_from_dict = Uom.from_dict(uom_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


