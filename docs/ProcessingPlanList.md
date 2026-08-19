# ProcessingPlanList

Список Техкарт

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ProcessingPlan]**](ProcessingPlan.md) | Массив Техкарт | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_plan_list import ProcessingPlanList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingPlanList from a JSON string
processing_plan_list_instance = ProcessingPlanList.from_json(json)
# print the JSON string representation of the object
print(ProcessingPlanList.to_json())

# convert the object into a dict
processing_plan_list_dict = processing_plan_list_instance.to_dict()
# create an instance of ProcessingPlanList from a dict
processing_plan_list_from_dict = ProcessingPlanList.from_dict(processing_plan_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


