# EmployeeList

Список сотрудников

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Employee]**](Employee.md) | Массив сотрудников | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.employee_list import EmployeeList

# TODO update the JSON string below
json = "{}"
# create an instance of EmployeeList from a JSON string
employee_list_instance = EmployeeList.from_json(json)
# print the JSON string representation of the object
print(EmployeeList.to_json())

# convert the object into a dict
employee_list_dict = employee_list_instance.to_dict()
# create an instance of EmployeeList from a dict
employee_list_from_dict = EmployeeList.from_dict(employee_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


