# ProcessingPlanFolderList

Список групп техкарт

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ProcessingPlanFolder]**](ProcessingPlanFolder.md) | Массив групп техкарт | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_plan_folder_list import ProcessingPlanFolderList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingPlanFolderList from a JSON string
processing_plan_folder_list_instance = ProcessingPlanFolderList.from_json(json)
# print the JSON string representation of the object
print(ProcessingPlanFolderList.to_json())

# convert the object into a dict
processing_plan_folder_list_dict = processing_plan_folder_list_instance.to_dict()
# create an instance of ProcessingPlanFolderList from a dict
processing_plan_folder_list_from_dict = ProcessingPlanFolderList.from_dict(processing_plan_folder_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


