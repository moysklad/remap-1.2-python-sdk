# MovePosition

Позиция Перемещения

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации, которую представляет собой позиция | [optional] 
**overhead** | **int** | Накладные расходы по позиции. Если позиции Перемещения не заданы, накладные расходы на уровне документа задать нельзя.  | [optional] [readonly] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**quantity** | **float** | Количество товаров/услуг данного вида в позиции. Если позиция — товар с учётом по серийным номерам, значение всегда равно количеству серийных номеров для этой позиции в документе.  | [optional] 
**source_slot** | [**StoreSlot**](StoreSlot.md) | Ячейка на складе, с которого совершается перемещение | [optional] 
**target_slot** | [**StoreSlot**](StoreSlot.md) | Ячейка на складе, на который совершается перемещение | [optional] 
**things** | **List[str]** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.move_position import MovePosition

# TODO update the JSON string below
json = "{}"
# create an instance of MovePosition from a JSON string
move_position_instance = MovePosition.from_json(json)
# print the JSON string representation of the object
print(MovePosition.to_json())

# convert the object into a dict
move_position_dict = move_position_instance.to_dict()
# create an instance of MovePosition from a dict
move_position_from_dict = MovePosition.from_dict(move_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


