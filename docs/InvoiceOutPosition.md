# InvoiceOutPosition

Позиция Счета покупателю

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**quantity** | **float** | Количество товаров/услуг данного вида в позиции | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**discount** | **float** | Процент скидки или наценки | [optional] 
**vat** | **int** | НДС, которым облагается текущая позиция | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для позиции | [optional] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации/комплекта, которую представляет собой позиция | [optional] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.invoice_out_position import InvoiceOutPosition

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceOutPosition from a JSON string
invoice_out_position_instance = InvoiceOutPosition.from_json(json)
# print the JSON string representation of the object
print(InvoiceOutPosition.to_json())

# convert the object into a dict
invoice_out_position_dict = invoice_out_position_instance.to_dict()
# create an instance of InvoiceOutPosition from a dict
invoice_out_position_from_dict = InvoiceOutPosition.from_dict(invoice_out_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


