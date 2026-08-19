# ProcessingOrderList

Список Заказов на производство

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ProcessingOrder]**](ProcessingOrder.md) | Массив Заказов на производство | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_order_list import ProcessingOrderList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingOrderList from a JSON string
processing_order_list_instance = ProcessingOrderList.from_json(json)
# print the JSON string representation of the object
print(ProcessingOrderList.to_json())

# convert the object into a dict
processing_order_list_dict = processing_order_list_instance.to_dict()
# create an instance of ProcessingOrderList from a dict
processing_order_list_from_dict = ProcessingOrderList.from_dict(processing_order_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


