# EnterPositionList

Список позиций Оприходования

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[EnterPosition]**](EnterPosition.md) | Массив позиций Оприходования | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.enter_position_list import EnterPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of EnterPositionList from a JSON string
enter_position_list_instance = EnterPositionList.from_json(json)
# print the JSON string representation of the object
print(EnterPositionList.to_json())

# convert the object into a dict
enter_position_list_dict = enter_position_list_instance.to_dict()
# create an instance of EnterPositionList from a dict
enter_position_list_from_dict = EnterPositionList.from_dict(enter_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


