# ProcessingProcessPosition

Позиция Техпроцесса

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**processingstage** | [**ProcessingStage**](ProcessingStage.md) |  | [optional] 
**next_positions** | [**List[ProcessingProcessPositionNextPositionsInner]**](ProcessingProcessPositionNextPositionsInner.md) | Метаданные следующих позиций позиции Техпроцесса | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_process_position import ProcessingProcessPosition

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingProcessPosition from a JSON string
processing_process_position_instance = ProcessingProcessPosition.from_json(json)
# print the JSON string representation of the object
print(ProcessingProcessPosition.to_json())

# convert the object into a dict
processing_process_position_dict = processing_process_position_instance.to_dict()
# create an instance of ProcessingProcessPosition from a dict
processing_process_position_from_dict = ProcessingProcessPosition.from_dict(processing_process_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


