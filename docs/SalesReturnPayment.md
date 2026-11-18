# SalesReturnPayment

Элемент массива `payments` документа salesReturn. Ссылка или раскрытый платеж; `linkedSum` может отсутствовать. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 
**linked_sum** | **float** | Сумма, оплаченная по данному документу; может отсутствовать у ссылки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.sales_return_payment import SalesReturnPayment

# TODO update the JSON string below
json = "{}"
# create an instance of SalesReturnPayment from a JSON string
sales_return_payment_instance = SalesReturnPayment.from_json(json)
# print the JSON string representation of the object
print(SalesReturnPayment.to_json())

# convert the object into a dict
sales_return_payment_dict = sales_return_payment_instance.to_dict()
# create an instance of SalesReturnPayment from a dict
sales_return_payment_from_dict = SalesReturnPayment.from_dict(sales_return_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


