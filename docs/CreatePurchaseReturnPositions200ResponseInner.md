# CreatePurchaseReturnPositions200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации, которую представляет собой позиция | [optional] 
**discount** | **float** | Процент скидки или наценки | [optional] [readonly] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**quantity** | **float** | Количество товаров данного вида в позиции | [optional] 
**slot** | [**StoreSlot**](StoreSlot.md) | Ячейка на складе | [optional] 
**things** | **List[str]** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  | [optional] 
**vat** | **int** | НДС, которым облагается текущая позиция | [optional] 
**vat_enabled** | **bool** | Включён ли НДС для позиции. Пара &#x60;(vat &#x3D; 0, vatEnabled &#x3D; false)&#x60; соответствует НДС «без НДС»; &#x60;(vat &#x3D; 0, vatEnabled &#x3D; true)&#x60; — НДС 0%.  | [optional] 
**errors** | [**List[Error]**](Error.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_purchase_return_positions200_response_inner import CreatePurchaseReturnPositions200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePurchaseReturnPositions200ResponseInner from a JSON string
create_purchase_return_positions200_response_inner_instance = CreatePurchaseReturnPositions200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreatePurchaseReturnPositions200ResponseInner.to_json())

# convert the object into a dict
create_purchase_return_positions200_response_inner_dict = create_purchase_return_positions200_response_inner_instance.to_dict()
# create an instance of CreatePurchaseReturnPositions200ResponseInner from a dict
create_purchase_return_positions200_response_inner_from_dict = CreatePurchaseReturnPositions200ResponseInner.from_dict(create_purchase_return_positions200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


