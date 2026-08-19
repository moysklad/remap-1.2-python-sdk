# MovePositionList

Список позиций Перемещения

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[MovePosition]**](MovePosition.md) | Массив позиций Перемещения | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.move_position_list import MovePositionList

# TODO update the JSON string below
json = "{}"
# create an instance of MovePositionList from a JSON string
move_position_list_instance = MovePositionList.from_json(json)
# print the JSON string representation of the object
print(MovePositionList.to_json())

# convert the object into a dict
move_position_list_dict = move_position_list_instance.to_dict()
# create an instance of MovePositionList from a dict
move_position_list_from_dict = MovePositionList.from_dict(move_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


