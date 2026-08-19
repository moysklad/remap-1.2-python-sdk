# DeleteInfo

Результат удаления сущности

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**info** | **str** | Информационное сообщение об удалении сущности | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.delete_info import DeleteInfo

# TODO update the JSON string below
json = "{}"
# create an instance of DeleteInfo from a JSON string
delete_info_instance = DeleteInfo.from_json(json)
# print the JSON string representation of the object
print(DeleteInfo.to_json())

# convert the object into a dict
delete_info_dict = delete_info_instance.to_dict()
# create an instance of DeleteInfo from a dict
delete_info_from_dict = DeleteInfo.from_dict(delete_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


