# ReportProfitByEmployeeList

Отчет «Прибыльность по сотрудникам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ReportProfitByEmployee]**](ReportProfitByEmployee.md) | Массив строк отчета прибыльности по сотрудникам | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_profit_by_employee_list import ReportProfitByEmployeeList

# TODO update the JSON string below
json = "{}"
# create an instance of ReportProfitByEmployeeList from a JSON string
report_profit_by_employee_list_instance = ReportProfitByEmployeeList.from_json(json)
# print the JSON string representation of the object
print(ReportProfitByEmployeeList.to_json())

# convert the object into a dict
report_profit_by_employee_list_dict = report_profit_by_employee_list_instance.to_dict()
# create an instance of ReportProfitByEmployeeList from a dict
report_profit_by_employee_list_from_dict = ReportProfitByEmployeeList.from_dict(report_profit_by_employee_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


