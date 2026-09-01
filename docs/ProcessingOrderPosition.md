# ProcessingOrderPosition

Позиция Заказа на производство

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**quantity** | **float** | Количество товаров данного вида в позиции | [optional] 
**reserve** | **float** | Резерв данной позиции | [optional] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации позиции | [optional] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_order_position import ProcessingOrderPosition

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingOrderPosition from a JSON string
processing_order_position_instance = ProcessingOrderPosition.from_json(json)
# print the JSON string representation of the object
print(ProcessingOrderPosition.to_json())

# convert the object into a dict
processing_order_position_dict = processing_order_position_instance.to_dict()
# create an instance of ProcessingOrderPosition from a dict
processing_order_position_from_dict = ProcessingOrderPosition.from_dict(processing_order_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


