# FinanceInOperationAbstract

Элемент массива `operations` приходного ордера / входящего платежа.  Допустимые `meta.type`: customerorder, purchasereturn, demand, invoiceout, commissionreportin, retailshift. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**linked_sum** | **float** | Сумма, оплаченная по данному документу | 

## Example

```python
from moysklad_remap_12_sdk.models.finance_in_operation_abstract import FinanceInOperationAbstract

# TODO update the JSON string below
json = "{}"
# create an instance of FinanceInOperationAbstract from a JSON string
finance_in_operation_abstract_instance = FinanceInOperationAbstract.from_json(json)
# print the JSON string representation of the object
print(FinanceInOperationAbstract.to_json())

# convert the object into a dict
finance_in_operation_abstract_dict = finance_in_operation_abstract_instance.to_dict()
# create an instance of FinanceInOperationAbstract from a dict
finance_in_operation_abstract_from_dict = FinanceInOperationAbstract.from_dict(finance_in_operation_abstract_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


