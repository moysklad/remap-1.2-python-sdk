# ProcessingProcessList

Список Техпроцессов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ProcessingProcess]**](ProcessingProcess.md) | Массив Техпроцессов | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_process_list import ProcessingProcessList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingProcessList from a JSON string
processing_process_list_instance = ProcessingProcessList.from_json(json)
# print the JSON string representation of the object
print(ProcessingProcessList.to_json())

# convert the object into a dict
processing_process_list_dict = processing_process_list_instance.to_dict()
# create an instance of ProcessingProcessList from a dict
processing_process_list_from_dict = ProcessingProcessList.from_dict(processing_process_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


