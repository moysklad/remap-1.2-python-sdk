# ActivateEmployeeRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**login** | **str** | Логин сотрудника (обязателен при первой активации) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**role** | [**EmployeeRole**](EmployeeRole.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.activate_employee_request import ActivateEmployeeRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ActivateEmployeeRequest from a JSON string
activate_employee_request_instance = ActivateEmployeeRequest.from_json(json)
# print the JSON string representation of the object
print(ActivateEmployeeRequest.to_json())

# convert the object into a dict
activate_employee_request_dict = activate_employee_request_instance.to_dict()
# create an instance of ActivateEmployeeRequest from a dict
activate_employee_request_from_dict = ActivateEmployeeRequest.from_dict(activate_employee_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


