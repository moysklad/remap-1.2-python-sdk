# ProcessingStageList

Список Этапов производства

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ProcessingStage]**](ProcessingStage.md) | Массив Этапов производства | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_stage_list import ProcessingStageList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingStageList from a JSON string
processing_stage_list_instance = ProcessingStageList.from_json(json)
# print the JSON string representation of the object
print(ProcessingStageList.to_json())

# convert the object into a dict
processing_stage_list_dict = processing_stage_list_instance.to_dict()
# create an instance of ProcessingStageList from a dict
processing_stage_list_from_dict = ProcessingStageList.from_dict(processing_stage_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


