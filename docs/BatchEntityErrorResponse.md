# BatchEntityErrorResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**errors** | [**List[Error]**](Error.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.batch_entity_error_response import BatchEntityErrorResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BatchEntityErrorResponse from a JSON string
batch_entity_error_response_instance = BatchEntityErrorResponse.from_json(json)
# print the JSON string representation of the object
print(BatchEntityErrorResponse.to_json())

# convert the object into a dict
batch_entity_error_response_dict = batch_entity_error_response_instance.to_dict()
# create an instance of BatchEntityErrorResponse from a dict
batch_entity_error_response_from_dict = BatchEntityErrorResponse.from_dict(batch_entity_error_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


