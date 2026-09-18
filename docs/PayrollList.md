# PayrollList

Список Начислений зарплаты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Payroll]**](Payroll.md) | Массив Начислений зарплаты | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.payroll_list import PayrollList

# TODO update the JSON string below
json = "{}"
# create an instance of PayrollList from a JSON string
payroll_list_instance = PayrollList.from_json(json)
# print the JSON string representation of the object
print(PayrollList.to_json())

# convert the object into a dict
payroll_list_dict = payroll_list_instance.to_dict()
# create an instance of PayrollList from a dict
payroll_list_from_dict = PayrollList.from_dict(payroll_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


