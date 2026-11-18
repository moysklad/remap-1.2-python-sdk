# BatchDeleteErrorResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**errors** | [**List[Error]**](Error.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.batch_delete_error_response import BatchDeleteErrorResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BatchDeleteErrorResponse from a JSON string
batch_delete_error_response_instance = BatchDeleteErrorResponse.from_json(json)
# print the JSON string representation of the object
print(BatchDeleteErrorResponse.to_json())

# convert the object into a dict
batch_delete_error_response_dict = batch_delete_error_response_instance.to_dict()
# create an instance of BatchDeleteErrorResponse from a dict
batch_delete_error_response_from_dict = BatchDeleteErrorResponse.from_dict(batch_delete_error_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


