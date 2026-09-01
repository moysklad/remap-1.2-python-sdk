# InventoryPosition

Позиция Инвентаризации

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации, которую представляет собой позиция | [optional] 
**calculated_quantity** | **float** | Расчетный остаток | [optional] 
**correction_amount** | **float** | Разница между расчетным остатком и фактическим | [optional] [readonly] 
**correction_sum** | **float** | Избыток/недостача | [optional] [readonly] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**things** | **List[str]** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  | [optional] 
**quantity** | **float** | Количество товаров/услуг данного вида в позиции. Если позиция - товар,  у которого включен учет по серийным номерам, то значение в этом поле всегда  будет равно количеству серийных номеров для данной позиции в документе.  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.inventory_position import InventoryPosition

# TODO update the JSON string below
json = "{}"
# create an instance of InventoryPosition from a JSON string
inventory_position_instance = InventoryPosition.from_json(json)
# print the JSON string representation of the object
print(InventoryPosition.to_json())

# convert the object into a dict
inventory_position_dict = inventory_position_instance.to_dict()
# create an instance of InventoryPosition from a dict
inventory_position_from_dict = InventoryPosition.from_dict(inventory_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


