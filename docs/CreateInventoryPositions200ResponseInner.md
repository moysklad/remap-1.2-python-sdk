# CreateInventoryPositions200ResponseInner


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
**errors** | [**List[Error]**](Error.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_inventory_positions200_response_inner import CreateInventoryPositions200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateInventoryPositions200ResponseInner from a JSON string
create_inventory_positions200_response_inner_instance = CreateInventoryPositions200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreateInventoryPositions200ResponseInner.to_json())

# convert the object into a dict
create_inventory_positions200_response_inner_dict = create_inventory_positions200_response_inner_instance.to_dict()
# create an instance of CreateInventoryPositions200ResponseInner from a dict
create_inventory_positions200_response_inner_from_dict = CreateInventoryPositions200ResponseInner.from_dict(create_inventory_positions200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


