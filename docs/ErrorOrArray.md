# ErrorOrArray


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**errors** | [**List[ErrorErrorsInner]**](ErrorErrorsInner.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.error_or_array import ErrorOrArray

# TODO update the JSON string below
json = "{}"
# create an instance of ErrorOrArray from a JSON string
error_or_array_instance = ErrorOrArray.from_json(json)
# print the JSON string representation of the object
print(ErrorOrArray.to_json())

# convert the object into a dict
error_or_array_dict = error_or_array_instance.to_dict()
# create an instance of ErrorOrArray from a dict
error_or_array_from_dict = ErrorOrArray.from_dict(error_or_array_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


