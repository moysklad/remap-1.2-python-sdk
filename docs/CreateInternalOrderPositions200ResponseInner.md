# CreateInternalOrderPositions200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**quantity** | **float** | Количество товаров данного вида в позиции | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**vat** | **int** | НДС, которым облагается текущая позиция | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для позиции | [optional] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/модификации/комплекта, которую представляет собой позиция | [optional] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 
**errors** | [**List[ErrorErrorsInner]**](ErrorErrorsInner.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_internal_order_positions200_response_inner import CreateInternalOrderPositions200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateInternalOrderPositions200ResponseInner from a JSON string
create_internal_order_positions200_response_inner_instance = CreateInternalOrderPositions200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreateInternalOrderPositions200ResponseInner.to_json())

# convert the object into a dict
create_internal_order_positions200_response_inner_dict = create_internal_order_positions200_response_inner_instance.to_dict()
# create an instance of CreateInternalOrderPositions200ResponseInner from a dict
create_internal_order_positions200_response_inner_from_dict = CreateInternalOrderPositions200ResponseInner.from_dict(create_internal_order_positions200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


