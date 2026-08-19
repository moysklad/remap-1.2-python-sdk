# ProcessingList

Список техопераций

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Processing]**](Processing.md) | Массив техопераций | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_list import ProcessingList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingList from a JSON string
processing_list_instance = ProcessingList.from_json(json)
# print the JSON string representation of the object
print(ProcessingList.to_json())

# convert the object into a dict
processing_list_dict = processing_list_instance.to_dict()
# create an instance of ProcessingList from a dict
processing_list_from_dict = ProcessingList.from_dict(processing_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


