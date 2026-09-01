# CreateProcessingOrderPositions200ResponseInner


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
**errors** | [**List[Error]**](Error.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_processing_order_positions200_response_inner import CreateProcessingOrderPositions200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateProcessingOrderPositions200ResponseInner from a JSON string
create_processing_order_positions200_response_inner_instance = CreateProcessingOrderPositions200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreateProcessingOrderPositions200ResponseInner.to_json())

# convert the object into a dict
create_processing_order_positions200_response_inner_dict = create_processing_order_positions200_response_inner_instance.to_dict()
# create an instance of CreateProcessingOrderPositions200ResponseInner from a dict
create_processing_order_positions200_response_inner_from_dict = CreateProcessingOrderPositions200ResponseInner.from_dict(create_processing_order_positions200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


