# EmissionOrderList

Список Заказов кодов маркировки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[EmissionOrder]**](EmissionOrder.md) | Массив Заказов кодов маркировки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.emission_order_list import EmissionOrderList

# TODO update the JSON string below
json = "{}"
# create an instance of EmissionOrderList from a JSON string
emission_order_list_instance = EmissionOrderList.from_json(json)
# print the JSON string representation of the object
print(EmissionOrderList.to_json())

# convert the object into a dict
emission_order_list_dict = emission_order_list_instance.to_dict()
# create an instance of EmissionOrderList from a dict
emission_order_list_from_dict = EmissionOrderList.from_dict(emission_order_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


