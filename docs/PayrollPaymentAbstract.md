# PayrollPaymentAbstract

Связанный платеж Начисления зарплаты с суммой оплаты `linkedSum`. Допустимые `meta.type`: paymentout, cashout. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**linked_sum** | **float** | Сумма, оплаченная по данному документу | 

## Example

```python
from moysklad_remap_12_sdk.models.payroll_payment_abstract import PayrollPaymentAbstract

# TODO update the JSON string below
json = "{}"
# create an instance of PayrollPaymentAbstract from a JSON string
payroll_payment_abstract_instance = PayrollPaymentAbstract.from_json(json)
# print the JSON string representation of the object
print(PayrollPaymentAbstract.to_json())

# convert the object into a dict
payroll_payment_abstract_dict = payroll_payment_abstract_instance.to_dict()
# create an instance of PayrollPaymentAbstract from a dict
payroll_payment_abstract_from_dict = PayrollPaymentAbstract.from_dict(payroll_payment_abstract_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


