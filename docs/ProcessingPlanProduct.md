# ProcessingPlanProduct

Продукт Техкарты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID продукта Техкарты | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) |  | [optional] 
**product** | [**Product**](Product.md) |  | [optional] 
**quantity** | **float** | Количество товаров данного вида в позиции | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_plan_product import ProcessingPlanProduct

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingPlanProduct from a JSON string
processing_plan_product_instance = ProcessingPlanProduct.from_json(json)
# print the JSON string representation of the object
print(ProcessingPlanProduct.to_json())

# convert the object into a dict
processing_plan_product_dict = processing_plan_product_instance.to_dict()
# create an instance of ProcessingPlanProduct from a dict
processing_plan_product_from_dict = ProcessingPlanProduct.from_dict(processing_plan_product_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


