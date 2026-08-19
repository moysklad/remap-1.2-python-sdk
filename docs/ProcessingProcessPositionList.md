# ProcessingProcessPositionList

Список позиций Техпроцесса

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ProcessingProcessPosition]**](ProcessingProcessPosition.md) | Массив позиций Техпроцесса | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_process_position_list import ProcessingProcessPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingProcessPositionList from a JSON string
processing_process_position_list_instance = ProcessingProcessPositionList.from_json(json)
# print the JSON string representation of the object
print(ProcessingProcessPositionList.to_json())

# convert the object into a dict
processing_process_position_list_dict = processing_process_position_list_instance.to_dict()
# create an instance of ProcessingProcessPositionList from a dict
processing_process_position_list_from_dict = ProcessingProcessPositionList.from_dict(processing_process_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


