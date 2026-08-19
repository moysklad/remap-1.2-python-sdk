# InternalOrderPositionList

Список позиций Внутреннего заказа

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[InternalOrderPosition]**](InternalOrderPosition.md) | Массив позиций Внутреннего заказа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.internal_order_position_list import InternalOrderPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of InternalOrderPositionList from a JSON string
internal_order_position_list_instance = InternalOrderPositionList.from_json(json)
# print the JSON string representation of the object
print(InternalOrderPositionList.to_json())

# convert the object into a dict
internal_order_position_list_dict = internal_order_position_list_instance.to_dict()
# create an instance of InternalOrderPositionList from a dict
internal_order_position_list_from_dict = InternalOrderPositionList.from_dict(internal_order_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


