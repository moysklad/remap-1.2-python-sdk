# ProcessingPlanMaterial

Материал Техкарты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID материала Техкарты | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) |  | [optional] 
**product** | [**Product**](Product.md) |  | [optional] 
**quantity** | **float** | Количество товаров данного вида в позиции | [optional] 
**processing_process_position** | [**ProcessingProcessPosition**](ProcessingProcessPosition.md) |  | [optional] 
**material_processing_plan** | [**ProcessingPlan**](ProcessingPlan.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_plan_material import ProcessingPlanMaterial

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingPlanMaterial from a JSON string
processing_plan_material_instance = ProcessingPlanMaterial.from_json(json)
# print the JSON string representation of the object
print(ProcessingPlanMaterial.to_json())

# convert the object into a dict
processing_plan_material_dict = processing_plan_material_instance.to_dict()
# create an instance of ProcessingPlanMaterial from a dict
processing_plan_material_from_dict = ProcessingPlanMaterial.from_dict(processing_plan_material_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


