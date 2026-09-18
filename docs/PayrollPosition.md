# PayrollPosition

Позиция Начисления зарплаты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**employee** | [**Employee**](Employee.md) |  | [optional] 
**base_salary** | **float** | Начисления по окладу сотрудника | [optional] 
**piecework_salary** | **float** | Начисления сдельной оплаты сотрудника | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.payroll_position import PayrollPosition

# TODO update the JSON string below
json = "{}"
# create an instance of PayrollPosition from a JSON string
payroll_position_instance = PayrollPosition.from_json(json)
# print the JSON string representation of the object
print(PayrollPosition.to_json())

# convert the object into a dict
payroll_position_dict = payroll_position_instance.to_dict()
# create an instance of PayrollPosition from a dict
payroll_position_from_dict = PayrollPosition.from_dict(payroll_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


