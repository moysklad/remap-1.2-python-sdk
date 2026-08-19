# Employee

Сотрудник

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID сотрудника | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование сотрудника | [optional] [readonly] 
**external_code** | **str** | Внешний код сотрудника | [optional] 
**archived** | **bool** | Добавлен ли сотрудник в архив | [optional] 
**created** | **str** | Момент создания | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления | [optional] [readonly] 
**description** | **str** | Комментарий к сотруднику | [optional] 
**email** | **str** | Адрес электронной почты | [optional] 
**phone** | **str** | Номер телефона | [optional] 
**first_name** | **str** | Имя | [optional] 
**middle_name** | **str** | Отчество | [optional] 
**last_name** | **str** | Фамилия | [optional] 
**full_name** | **str** | Полное имя сотрудника | [optional] [readonly] 
**short_fio** | **str** | Краткое ФИО сотрудника | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**inn** | **str** | ИНН сотрудника (в формате ИНН физического лица) | [optional] 
**position** | **str** | Должность сотрудника | [optional] 
**uid** | **str** | Логин сотрудника | [optional] [readonly] 
**salary** | [**EmployeeSalary**](EmployeeSalary.md) |  | [optional] 
**cashiers** | [**List[Cashier]**](Cashier.md) | Массив кассиров | [optional] [readonly] 
**image** | [**Image**](Image.md) | Фотография сотрудника | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Дополнительные поля | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.employee import Employee

# TODO update the JSON string below
json = "{}"
# create an instance of Employee from a JSON string
employee_instance = Employee.from_json(json)
# print the JSON string representation of the object
print(Employee.to_json())

# convert the object into a dict
employee_dict = employee_instance.to_dict()
# create an instance of Employee from a dict
employee_from_dict = Employee.from_dict(employee_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


