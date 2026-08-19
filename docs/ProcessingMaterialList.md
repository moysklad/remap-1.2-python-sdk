# ProcessingMaterialList

Список материалов техоперации

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ProcessingMaterial]**](ProcessingMaterial.md) | Массив материалов техоперации | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_material_list import ProcessingMaterialList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingMaterialList from a JSON string
processing_material_list_instance = ProcessingMaterialList.from_json(json)
# print the JSON string representation of the object
print(ProcessingMaterialList.to_json())

# convert the object into a dict
processing_material_list_dict = processing_material_list_instance.to_dict()
# create an instance of ProcessingMaterialList from a dict
processing_material_list_from_dict = ProcessingMaterialList.from_dict(processing_material_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


