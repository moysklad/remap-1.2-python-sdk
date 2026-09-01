# InternalOrderPosition

Позиция Внутреннего заказа

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**quantity** | **float** | Количество товаров данного вида в позиции | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**vat** | **int** | НДС, которым облагается текущая позиция | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для позиции | [optional] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/модификации/комплекта, которую представляет собой позиция | [optional] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.internal_order_position import InternalOrderPosition

# TODO update the JSON string below
json = "{}"
# create an instance of InternalOrderPosition from a JSON string
internal_order_position_instance = InternalOrderPosition.from_json(json)
# print the JSON string representation of the object
print(InternalOrderPosition.to_json())

# convert the object into a dict
internal_order_position_dict = internal_order_position_instance.to_dict()
# create an instance of InternalOrderPosition from a dict
internal_order_position_from_dict = InternalOrderPosition.from_dict(internal_order_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


