# CreateInvoiceInPositionsBatch200ResponseInner


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
**errors** | [**List[Error]**](Error.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_invoice_in_positions_batch200_response_inner import CreateInvoiceInPositionsBatch200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateInvoiceInPositionsBatch200ResponseInner from a JSON string
create_invoice_in_positions_batch200_response_inner_instance = CreateInvoiceInPositionsBatch200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreateInvoiceInPositionsBatch200ResponseInner.to_json())

# convert the object into a dict
create_invoice_in_positions_batch200_response_inner_dict = create_invoice_in_positions_batch200_response_inner_instance.to_dict()
# create an instance of CreateInvoiceInPositionsBatch200ResponseInner from a dict
create_invoice_in_positions_batch200_response_inner_from_dict = CreateInvoiceInPositionsBatch200ResponseInner.from_dict(create_invoice_in_positions_batch200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


