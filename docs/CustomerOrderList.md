# CustomerOrderList

Список Заказов покупателей

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[CustomerOrder]**](CustomerOrder.md) | Массив Заказов покупателей | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.customer_order_list import CustomerOrderList

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerOrderList from a JSON string
customer_order_list_instance = CustomerOrderList.from_json(json)
# print the JSON string representation of the object
print(CustomerOrderList.to_json())

# convert the object into a dict
customer_order_list_dict = customer_order_list_instance.to_dict()
# create an instance of CustomerOrderList from a dict
customer_order_list_from_dict = CustomerOrderList.from_dict(customer_order_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


