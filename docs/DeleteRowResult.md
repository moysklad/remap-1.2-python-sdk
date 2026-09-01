# DeleteRowResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**info** | **str** | Информационное сообщение об удалении сущности | [optional] 
**errors** | [**List[Error]**](Error.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.delete_row_result import DeleteRowResult

# TODO update the JSON string below
json = "{}"
# create an instance of DeleteRowResult from a JSON string
delete_row_result_instance = DeleteRowResult.from_json(json)
# print the JSON string representation of the object
print(DeleteRowResult.to_json())

# convert the object into a dict
delete_row_result_dict = delete_row_result_instance.to_dict()
# create an instance of DeleteRowResult from a dict
delete_row_result_from_dict = DeleteRowResult.from_dict(delete_row_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


