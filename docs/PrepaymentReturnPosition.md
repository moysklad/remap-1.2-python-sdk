# PrepaymentReturnPosition

Позиция Возврата предоплаты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации, которую представляет собой позиция | [optional] 
**discount** | **float** | Процент скидки или наценки | [optional] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**quantity** | **float** | Количество товаров/услуг данного вида в позиции. | [optional] 
**vat** | **int** | НДС, которым облагается текущая позиция | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для позиции | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.prepayment_return_position import PrepaymentReturnPosition

# TODO update the JSON string below
json = "{}"
# create an instance of PrepaymentReturnPosition from a JSON string
prepayment_return_position_instance = PrepaymentReturnPosition.from_json(json)
# print the JSON string representation of the object
print(PrepaymentReturnPosition.to_json())

# convert the object into a dict
prepayment_return_position_dict = prepayment_return_position_instance.to_dict()
# create an instance of PrepaymentReturnPosition from a dict
prepayment_return_position_from_dict = PrepaymentReturnPosition.from_dict(prepayment_return_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


