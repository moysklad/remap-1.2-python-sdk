# CustomerOrderPositionList

Список позиций Заказа покупателя

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[CustomerOrderPosition]**](CustomerOrderPosition.md) | Массив позиций Заказа покупателя | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.customer_order_position_list import CustomerOrderPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerOrderPositionList from a JSON string
customer_order_position_list_instance = CustomerOrderPositionList.from_json(json)
# print the JSON string representation of the object
print(CustomerOrderPositionList.to_json())

# convert the object into a dict
customer_order_position_list_dict = customer_order_position_list_instance.to_dict()
# create an instance of CustomerOrderPositionList from a dict
customer_order_position_list_from_dict = CustomerOrderPositionList.from_dict(customer_order_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


