# ProcessingPlanMetadata

Метаданные Техкарты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**attributes** | [**AttributeMetaInfoList**](AttributeMetaInfoList.md) |  | [optional] 
**create_shared** | **bool** | Создавать новые Техкарты с меткой \&quot;Общий\&quot; | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_plan_metadata import ProcessingPlanMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingPlanMetadata from a JSON string
processing_plan_metadata_instance = ProcessingPlanMetadata.from_json(json)
# print the JSON string representation of the object
print(ProcessingPlanMetadata.to_json())

# convert the object into a dict
processing_plan_metadata_dict = processing_plan_metadata_instance.to_dict()
# create an instance of ProcessingPlanMetadata from a dict
processing_plan_metadata_from_dict = ProcessingPlanMetadata.from_dict(processing_plan_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


