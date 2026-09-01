# InvoiceInPosition

Позиция Счета поставщику

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] 
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
from moysklad_remap_12_sdk.models.invoice_in_position import InvoiceInPosition

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceInPosition from a JSON string
invoice_in_position_instance = InvoiceInPosition.from_json(json)
# print the JSON string representation of the object
print(InvoiceInPosition.to_json())

# convert the object into a dict
invoice_in_position_dict = invoice_in_position_instance.to_dict()
# create an instance of InvoiceInPosition from a dict
invoice_in_position_from_dict = InvoiceInPosition.from_dict(invoice_in_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


