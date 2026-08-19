# EmployeeSecurity

Права сотрудника

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_active** | **bool** | Доступ к сервису МойСклад | [optional] 
**login** | **str** | Логин сотрудника для входа в МойСклад | [optional] 
**email** | **str** | Почта сотрудника | [optional] 
**group** | [**EmployeeSecurityGroup**](EmployeeSecurityGroup.md) |  | [optional] 
**authorized_hosts** | **List[str]** | Список ipv4 адресов, с которых разрешен доступ на аккаунт | [optional] 
**authorized_ip_network** | **str** | Ipv4 адрес, идентифицирующий соответствующую подсеть, с правом доступа на аккаунт | [optional] 
**authorized_ip_netmask** | **str** | Маска подсети с правом доступа на аккаунт | [optional] 
**role** | [**EmployeeRole**](EmployeeRole.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.employee_security import EmployeeSecurity

# TODO update the JSON string below
json = "{}"
# create an instance of EmployeeSecurity from a JSON string
employee_security_instance = EmployeeSecurity.from_json(json)
# print the JSON string representation of the object
print(EmployeeSecurity.to_json())

# convert the object into a dict
employee_security_dict = employee_security_instance.to_dict()
# create an instance of EmployeeSecurity from a dict
employee_security_from_dict = EmployeeSecurity.from_dict(employee_security_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


