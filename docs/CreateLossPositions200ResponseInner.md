# CreateLossPositions200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации, которую представляет собой позиция | [optional] 
**declaration** | [**List[DeclarationInner]**](DeclarationInner.md) | Информация о прослеживаемости импортных товаров. Не входит в ответ по умолчанию; может быть возвращена только при явном запросе &#x60;fields&#x3D;declaration&#x60;. Только для чтения.  | [optional] [readonly] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**quantity** | **float** | Количество товаров/услуг данного вида в позиции | [optional] 
**reason** | **str** | Причина списания данной позиции | [optional] 
**slot** | [**StoreSlot**](StoreSlot.md) | Ячейка на складе | [optional] 
**things** | **List[str]** | Серийные номера | [optional] 
**errors** | [**List[ErrorErrorsInner]**](ErrorErrorsInner.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_loss_positions200_response_inner import CreateLossPositions200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateLossPositions200ResponseInner from a JSON string
create_loss_positions200_response_inner_instance = CreateLossPositions200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreateLossPositions200ResponseInner.to_json())

# convert the object into a dict
create_loss_positions200_response_inner_dict = create_loss_positions200_response_inner_instance.to_dict()
# create an instance of CreateLossPositions200ResponseInner from a dict
create_loss_positions200_response_inner_from_dict = CreateLossPositions200ResponseInner.from_dict(create_loss_positions200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


