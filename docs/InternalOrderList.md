# InternalOrderList

Список Внутренних заказов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[InternalOrder]**](InternalOrder.md) | Массив Внутренних заказов | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.internal_order_list import InternalOrderList

# TODO update the JSON string below
json = "{}"
# create an instance of InternalOrderList from a JSON string
internal_order_list_instance = InternalOrderList.from_json(json)
# print the JSON string representation of the object
print(InternalOrderList.to_json())

# convert the object into a dict
internal_order_list_dict = internal_order_list_instance.to_dict()
# create an instance of InternalOrderList from a dict
internal_order_list_from_dict = InternalOrderList.from_dict(internal_order_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


