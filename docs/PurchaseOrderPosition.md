# PurchaseOrderPosition

Позиция Заказа поставщику

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**quantity** | **float** | Количество товаров данного вида в позиции | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**discount** | **float** | Процент скидки или наценки | [optional] 
**shipped** | **float** | Принято | [optional] [readonly] 
**in_transit** | **float** | Ожидание | [optional] [readonly] 
**vat** | **int** | НДС, которым облагается текущая позиция | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для позиции | [optional] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/модификации/партии, которую представляет собой позиция | [optional] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 
**stock** | [**PositionStock**](PositionStock.md) | Остатки и себестоимость позиции. Не выводится по умолчанию. Для получения передайте параметр &#x60;?fields&#x3D;stock&#x60;.  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.purchase_order_position import PurchaseOrderPosition

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseOrderPosition from a JSON string
purchase_order_position_instance = PurchaseOrderPosition.from_json(json)
# print the JSON string representation of the object
print(PurchaseOrderPosition.to_json())

# convert the object into a dict
purchase_order_position_dict = purchase_order_position_instance.to_dict()
# create an instance of PurchaseOrderPosition from a dict
purchase_order_position_from_dict = PurchaseOrderPosition.from_dict(purchase_order_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


