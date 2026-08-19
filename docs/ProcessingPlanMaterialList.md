# ProcessingPlanMaterialList

Список материалов Техкарты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ProcessingPlanMaterial]**](ProcessingPlanMaterial.md) | Массив материалов Техкарты | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_plan_material_list import ProcessingPlanMaterialList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingPlanMaterialList from a JSON string
processing_plan_material_list_instance = ProcessingPlanMaterialList.from_json(json)
# print the JSON string representation of the object
print(ProcessingPlanMaterialList.to_json())

# convert the object into a dict
processing_plan_material_list_dict = processing_plan_material_list_instance.to_dict()
# create an instance of ProcessingPlanMaterialList from a dict
processing_plan_material_list_from_dict = ProcessingPlanMaterialList.from_dict(processing_plan_material_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


