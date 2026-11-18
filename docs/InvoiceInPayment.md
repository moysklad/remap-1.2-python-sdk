# InvoiceInPayment

Элемент массива `payments` документа invoiceIn. Ссылка или раскрытый платеж; `linkedSum` может отсутствовать. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 
**linked_sum** | **float** | Сумма, оплаченная по данному документу; может отсутствовать у ссылки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.invoice_in_payment import InvoiceInPayment

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceInPayment from a JSON string
invoice_in_payment_instance = InvoiceInPayment.from_json(json)
# print the JSON string representation of the object
print(InvoiceInPayment.to_json())

# convert the object into a dict
invoice_in_payment_dict = invoice_in_payment_instance.to_dict()
# create an instance of InvoiceInPayment from a dict
invoice_in_payment_from_dict = InvoiceInPayment.from_dict(invoice_in_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


