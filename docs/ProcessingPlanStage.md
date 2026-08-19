# ProcessingPlanStage

Этап Техкарты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID этапа Техкарты | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**enable_hour_accounting** | **bool** | Признак активности учета по нормо-часам | [optional] 
**cost** | **float** | Стоимость производства на определенном этапе | [optional] 
**labour_cost** | **float** | Оплата труда на определенном этапе | [optional] 
**standard_hour** | **float** | Нормо-часы на определенном этапе | [optional] 
**standard_hour_cost** | **float** | Стоимость нормо-часа | [optional] [readonly] 
**processing_process_position** | [**ProcessingProcessPosition**](ProcessingProcessPosition.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_plan_stage import ProcessingPlanStage

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingPlanStage from a JSON string
processing_plan_stage_instance = ProcessingPlanStage.from_json(json)
# print the JSON string representation of the object
print(ProcessingPlanStage.to_json())

# convert the object into a dict
processing_plan_stage_dict = processing_plan_stage_instance.to_dict()
# create an instance of ProcessingPlanStage from a dict
processing_plan_stage_from_dict = ProcessingPlanStage.from_dict(processing_plan_stage_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


