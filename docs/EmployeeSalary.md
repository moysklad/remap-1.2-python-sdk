# EmployeeSalary

Оклад сотрудника

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **float** | Сумма оклада | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.employee_salary import EmployeeSalary

# TODO update the JSON string below
json = "{}"
# create an instance of EmployeeSalary from a JSON string
employee_salary_instance = EmployeeSalary.from_json(json)
# print the JSON string representation of the object
print(EmployeeSalary.to_json())

# convert the object into a dict
employee_salary_dict = employee_salary_instance.to_dict()
# create an instance of EmployeeSalary from a dict
employee_salary_from_dict = EmployeeSalary.from_dict(employee_salary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


