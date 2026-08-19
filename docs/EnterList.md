# EnterList

Список Оприходований

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Enter]**](Enter.md) | Массив Оприходований | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.enter_list import EnterList

# TODO update the JSON string below
json = "{}"
# create an instance of EnterList from a JSON string
enter_list_instance = EnterList.from_json(json)
# print the JSON string representation of the object
print(EnterList.to_json())

# convert the object into a dict
enter_list_dict = enter_list_instance.to_dict()
# create an instance of EnterList from a dict
enter_list_from_dict = EnterList.from_dict(enter_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


