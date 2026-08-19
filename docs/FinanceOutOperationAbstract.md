# FinanceOutOperationAbstract

Элемент массива `operations` расходного ордера / исходящего платежа: документ одного из допустимых типов плюс обязательное поле `linkedSum`.  Допустимые `meta.type`: salesreturn, supply, invoicein, purchaseorder, commissionreportout. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**linked_sum** | **float** | Сумма, оплаченная по данному документу | 

## Example

```python
from moysklad_remap_12_sdk.models.finance_out_operation_abstract import FinanceOutOperationAbstract

# TODO update the JSON string below
json = "{}"
# create an instance of FinanceOutOperationAbstract from a JSON string
finance_out_operation_abstract_instance = FinanceOutOperationAbstract.from_json(json)
# print the JSON string representation of the object
print(FinanceOutOperationAbstract.to_json())

# convert the object into a dict
finance_out_operation_abstract_dict = finance_out_operation_abstract_instance.to_dict()
# create an instance of FinanceOutOperationAbstract from a dict
finance_out_operation_abstract_from_dict = FinanceOutOperationAbstract.from_dict(finance_out_operation_abstract_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


