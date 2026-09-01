# PurchaseReturnPosition

Позиция Возврата поставщику

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

## Example

```python
from moysklad_remap_12_sdk.models.purchase_return_position import PurchaseReturnPosition

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseReturnPosition from a JSON string
purchase_return_position_instance = PurchaseReturnPosition.from_json(json)
# print the JSON string representation of the object
print(PurchaseReturnPosition.to_json())

# convert the object into a dict
purchase_return_position_dict = purchase_return_position_instance.to_dict()
# create an instance of PurchaseReturnPosition from a dict
purchase_return_position_from_dict = PurchaseReturnPosition.from_dict(purchase_return_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


