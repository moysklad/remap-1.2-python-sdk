# CustomerOrderPayment

Элемент массива `payments` документа customerOrder. Ссылка или раскрытый платеж; `linkedSum` может отсутствовать. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 
**linked_sum** | **float** | Сумма, оплаченная по данному документу; может отсутствовать у ссылки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.customer_order_payment import CustomerOrderPayment

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerOrderPayment from a JSON string
customer_order_payment_instance = CustomerOrderPayment.from_json(json)
# print the JSON string representation of the object
print(CustomerOrderPayment.to_json())

# convert the object into a dict
customer_order_payment_dict = customer_order_payment_instance.to_dict()
# create an instance of CustomerOrderPayment from a dict
customer_order_payment_from_dict = CustomerOrderPayment.from_dict(customer_order_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


