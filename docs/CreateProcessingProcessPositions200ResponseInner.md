# CreateProcessingProcessPositions200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**processingstage** | [**ProcessingStage**](ProcessingStage.md) |  | [optional] 
**next_positions** | [**List[ProcessingProcessPositionNextPositionsInner]**](ProcessingProcessPositionNextPositionsInner.md) | Метаданные следующих позиций позиции Техпроцесса | [optional] 
**errors** | [**List[Error]**](Error.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_processing_process_positions200_response_inner import CreateProcessingProcessPositions200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateProcessingProcessPositions200ResponseInner from a JSON string
create_processing_process_positions200_response_inner_instance = CreateProcessingProcessPositions200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreateProcessingProcessPositions200ResponseInner.to_json())

# convert the object into a dict
create_processing_process_positions200_response_inner_dict = create_processing_process_positions200_response_inner_instance.to_dict()
# create an instance of CreateProcessingProcessPositions200ResponseInner from a dict
create_processing_process_positions200_response_inner_from_dict = CreateProcessingProcessPositions200ResponseInner.from_dict(create_processing_process_positions200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


