# RetailShiftPaymentOperation

Элемент массива `paymentOperations` розничной смены.  Допустимые `meta.type`: cashin, paymentin. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**linked_sum** | **float** | Сумма, оплаченная по данному документу | 

## Example

```python
from moysklad_remap_12_sdk.models.retail_shift_payment_operation import RetailShiftPaymentOperation

# TODO update the JSON string below
json = "{}"
# create an instance of RetailShiftPaymentOperation from a JSON string
retail_shift_payment_operation_instance = RetailShiftPaymentOperation.from_json(json)
# print the JSON string representation of the object
print(RetailShiftPaymentOperation.to_json())

# convert the object into a dict
retail_shift_payment_operation_dict = retail_shift_payment_operation_instance.to_dict()
# create an instance of RetailShiftPaymentOperation from a dict
retail_shift_payment_operation_from_dict = RetailShiftPaymentOperation.from_dict(retail_shift_payment_operation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


