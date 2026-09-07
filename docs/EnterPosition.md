# EnterPosition

Позиция Оприходования

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации, которую представляет собой позиция | [optional] 
**country** | [**Country**](Country.md) | Метаданные страны | [optional] 
**gtd** | [**Gtd**](Gtd.md) |  | [optional] 
**overhead** | **float** | Накладные расходы | [optional] [readonly] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**quantity** | **float** | Количество товаров данного вида в позиции | [optional] 
**reason** | **str** | Причина оприходования данной позиции | [optional] 
**slot** | [**StoreSlot**](StoreSlot.md) | Ячейка на складе | [optional] 
**things** | **List[str]** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.enter_position import EnterPosition

# TODO update the JSON string below
json = "{}"
# create an instance of EnterPosition from a JSON string
enter_position_instance = EnterPosition.from_json(json)
# print the JSON string representation of the object
print(EnterPosition.to_json())

# convert the object into a dict
enter_position_dict = enter_position_instance.to_dict()
# create an instance of EnterPosition from a dict
enter_position_from_dict = EnterPosition.from_dict(enter_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


