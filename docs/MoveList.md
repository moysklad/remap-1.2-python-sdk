# MoveList

Список Перемещений

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Move]**](Move.md) | Массив Перемещений | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.move_list import MoveList

# TODO update the JSON string below
json = "{}"
# create an instance of MoveList from a JSON string
move_list_instance = MoveList.from_json(json)
# print the JSON string representation of the object
print(MoveList.to_json())

# convert the object into a dict
move_list_dict = move_list_instance.to_dict()
# create an instance of MoveList from a dict
move_list_from_dict = MoveList.from_dict(move_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


