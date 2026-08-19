# ProcessingPlanStageList

Список этапов Техкарты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ProcessingPlanStage]**](ProcessingPlanStage.md) | Массив этапов Техкарты | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_plan_stage_list import ProcessingPlanStageList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingPlanStageList from a JSON string
processing_plan_stage_list_instance = ProcessingPlanStageList.from_json(json)
# print the JSON string representation of the object
print(ProcessingPlanStageList.to_json())

# convert the object into a dict
processing_plan_stage_list_dict = processing_plan_stage_list_instance.to_dict()
# create an instance of ProcessingPlanStageList from a dict
processing_plan_stage_list_from_dict = ProcessingPlanStageList.from_dict(processing_plan_stage_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


