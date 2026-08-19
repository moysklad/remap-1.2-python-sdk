# ProcessingPlanProductList

Список продуктов Техкарты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ProcessingPlanProduct]**](ProcessingPlanProduct.md) | Массив продуктов Техкарты | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_plan_product_list import ProcessingPlanProductList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingPlanProductList from a JSON string
processing_plan_product_list_instance = ProcessingPlanProductList.from_json(json)
# print the JSON string representation of the object
print(ProcessingPlanProductList.to_json())

# convert the object into a dict
processing_plan_product_list_dict = processing_plan_product_list_instance.to_dict()
# create an instance of ProcessingPlanProductList from a dict
processing_plan_product_list_from_dict = ProcessingPlanProductList.from_dict(processing_plan_product_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


