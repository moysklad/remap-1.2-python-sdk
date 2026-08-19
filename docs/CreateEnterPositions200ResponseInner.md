# CreateEnterPositions200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации, которую представляет собой позиция | [optional] 
**country** | [**Country**](Country.md) | Метаданные страны | [optional] 
**gtd** | [**Gtd**](Gtd.md) |  | [optional] 
**overhead** | **int** | Накладные расходы | [optional] [readonly] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**quantity** | **float** | Количество товаров данного вида в позиции | [optional] 
**reason** | **str** | Причина оприходования данной позиции | [optional] 
**slot** | [**StoreSlot**](StoreSlot.md) | Ячейка на складе | [optional] 
**things** | **List[str]** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  | [optional] 
**errors** | [**List[ErrorErrorsInner]**](ErrorErrorsInner.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_enter_positions200_response_inner import CreateEnterPositions200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateEnterPositions200ResponseInner from a JSON string
create_enter_positions200_response_inner_instance = CreateEnterPositions200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreateEnterPositions200ResponseInner.to_json())

# convert the object into a dict
create_enter_positions200_response_inner_dict = create_enter_positions200_response_inner_instance.to_dict()
# create an instance of CreateEnterPositions200ResponseInner from a dict
create_enter_positions200_response_inner_from_dict = CreateEnterPositions200ResponseInner.from_dict(create_enter_positions200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


